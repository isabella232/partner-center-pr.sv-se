---
title: Skapa och hantera privata Azure Marketplace i Azure Portal
description: Lär dig mer om att skapa och hantera Azure Marketplace (förhandsversion) i Azure Portal. Med Azure Marketplace (förhandsversion) kan administratörer styra vilka lösningar från tredje part deras användare kan använda.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 9da9eb4944508e815d1664fb44b13bce52f37150
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431676"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="f8b8f-104">Skapa och hantera privata Azure Marketplace i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="f8b8f-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="f8b8f-105">Privata Azure Marketplace administratörer styra vilka lösningar från tredje part deras användare kan använda.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="f8b8f-106">Den gör detta genom att tillåta användaren att endast distribuera erbjudanden som har godkänts av administratören och som uppfyller företagets principer.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="f8b8f-107">Med Private Azure Marketplace kan användarna söka i onlinebutiken efter kompatibla erbjudanden att köpa och distribuera.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="f8b8f-108">Som Marketplace-administratör (tilldelad roll) börjar du med ett inaktiverat och tomt privat arkiv där du kan lägga till godkända erbjudanden och planer.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="f8b8f-109">Den här artikeln förklarar hur du tilldelar den roll som krävs, skapar ett privat arkiv, hanterar objekt, godkänner användarbegäranden och aktiverar privata Azure Marketplace för dina användare.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="f8b8f-110">Privata Azure Marketplace på klientorganisationsnivå, så alla användare under klientorganisationen ser samma curated lista.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="f8b8f-111">Alla Microsoft-lösningar (inklusive [godkända Linux-distributioner)](/azure/virtual-machines/linux/endorsed-distros)läggs automatiskt till i privata Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="f8b8f-112">Tilldela administratörsrollen för Marketplace</span><span class="sxs-lookup"><span data-stu-id="f8b8f-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="f8b8f-113">Klientorganisationen Global administratör tilldela Administratörsrollen **för Marketplace** till den privata Azure Marketplace som ska hantera det privata arkivet.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="f8b8f-114">Åtkomst till privat Azure Marketplace är endast tillgänglig för IT-administratörer med administratörsrollen Marketplace tilldelad.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="f8b8f-115">Förutsättningar</span><span class="sxs-lookup"><span data-stu-id="f8b8f-115">Prerequisites</span></span>

<span data-ttu-id="f8b8f-116">Dessa krav måste vara uppfyllda innan du kan tilldela administratörsrollen för Marketplace till en användare i klientorganisationsomfånget:</span><span class="sxs-lookup"><span data-stu-id="f8b8f-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="f8b8f-117">Du har åtkomst till en **Global administratör** användare.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="f8b8f-118">Klienten har minst en prenumeration (kan vara vilken typ som helst).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="f8b8f-119">Användaren Global administratör tilldelas rollen **Deltagare eller** högre för den valda prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="f8b8f-120">Tilldela administratörsrollen för Marketplace med åtkomstkontroll (IAM)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="f8b8f-121">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="f8b8f-122">Välj **Alla tjänster** och sedan **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="f8b8f-123">Välj **Privat Marketplace** på menyn till vänster.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="f8b8f-124">[![Visar menyalternativet privat marketplace till vänster på Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="f8b8f-125">Välj **Åtkomstkontroll (IAM) för** att tilldela administratörsrollen för Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Visar skärmen IA M-åtkomstkontroll.":::

1. <span data-ttu-id="f8b8f-127">Välj **+ Lägg till** > **Lägg till rolltilldelning**.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="f8b8f-128">Under **Roll** väljer du **Marketplace-administratör.**</span><span class="sxs-lookup"><span data-stu-id="f8b8f-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Visar menyn Rolltilldelning.":::

1. <span data-ttu-id="f8b8f-130">Välj önskad användare i listrutan och välj sedan **Klar.**</span><span class="sxs-lookup"><span data-stu-id="f8b8f-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="f8b8f-131">Tilldela administratörsrollen för Marketplace med PowerShell</span><span class="sxs-lookup"><span data-stu-id="f8b8f-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="f8b8f-132">Använd följande PowerShell-skript för att tilldela administratörsrollen för Marketplace: Det kräver följande parametrar:</span><span class="sxs-lookup"><span data-stu-id="f8b8f-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="f8b8f-133">**TenantId:** ID:t för klienten i omfånget (Marketplace-administratörsrollen kan tilldelas i klientorganisationsomfånget).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="f8b8f-134">**SubscriptionId:** En prenumeration som den globala administratören har rollen **Deltagare eller** högre tilldelad.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="f8b8f-135">**GlobalAdminUsername:** Användarnamnet för den globala administratören.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="f8b8f-136">**UsernameToAssignRoleFor:** Användarnamnet som administratörsrollen för Marketplace ska tilldelas.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="f8b8f-137">För gästanvändare som bjudits in till klientorganisationen kan det ta upp till 48 timmar innan deras konto är tillgängligt för tilldelning av rollen Marketplace-administratör.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="f8b8f-138">Mer information finns i Egenskaper [för en Azure Active Directory B2B-samarbetsanvändare](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="f8b8f-139">Mer information om cmdletarna i PowerShell-modulen Az.Portal finns i [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="f8b8f-140">Skapa privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f8b8f-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="f8b8f-141">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="f8b8f-142">Välj **Alla tjänster** och sedan **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Visar Azure Portal huvudfönstret.":::

3. <span data-ttu-id="f8b8f-144">Välj **Privat Marketplace** på menyn till vänster.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="f8b8f-145">Välj **Kom igång** för att skapa Azure Marketplace (du behöver bara göra det här en gång).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Visar hur du väljer huvudfönstret &quot;Kom igång Azure Portal&quot;.":::

    <span data-ttu-id="f8b8f-147">Om privat Azure Marketplace redan finns för den här klientorganisationen väljs Hantera **Marketplace** som standard.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="f8b8f-148">När det är klart har du en tom och inaktiverad privat Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Visar den tomma privata Azure Marketplace skärmen.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="f8b8f-150">Lägga till objekt från galleriet</span><span class="sxs-lookup"><span data-stu-id="f8b8f-150">Add items from gallery</span></span>

<span data-ttu-id="f8b8f-151">Ett objekt är en kombination av ett erbjudande och en plan.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="f8b8f-152">Du kan söka efter och lägga till objekt på sidan Hantera Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="f8b8f-153">Välj **Lägg till objekt.**</span><span class="sxs-lookup"><span data-stu-id="f8b8f-153">Select **Add items**.</span></span>

2. <span data-ttu-id="f8b8f-154">Bläddra i **galleriet** eller använd sökfältet för att hitta det objekt som du vill använda.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="f8b8f-155">[![Visar hur du bläddrar i galleriet eller använder sökfältet.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="f8b8f-156">När du lägger till ett nytt erbjudande läggs som standard alla aktuella planer till i listan över godkända planer.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="f8b8f-157">Om du vill ändra valet av plan innan du lägger till de valda objekten väljer du den nedrullningsna menyn i erbjudandets panel och uppdaterar de planer som krävs.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Visar hur du uppdaterar de planer som krävs.":::

4. <span data-ttu-id="f8b8f-159">Välj **Klar** längst ned till vänster när du har gjort dina val.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="f8b8f-160">**Lägg till** objekt på Marketplace kommer endast att vara tillgängligt för erbjudanden som inte kommer från Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="f8b8f-161">Microsoft-lösningar [(inklusive godkända Linux-distributioner)](/azure/virtual-machines/linux/endorsed-distros)taggas som "Godkända som standard" och kan inte hanteras på privat Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="f8b8f-162">Redigera objektplaner</span><span class="sxs-lookup"><span data-stu-id="f8b8f-162">Edit item's plans</span></span>

<span data-ttu-id="f8b8f-163">Du kan redigera ett objekts planer på sidan Hantera Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="f8b8f-164">Granska de **tillgängliga** planerna i den nedrullningsbara menyn för objektet i kolumnen Planer.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="f8b8f-165">Markera eller avmarkera kryssrutorna för att välja vilka planer som ska göras tillgängliga för användarna.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Visar hur du markerar eller avmarkerar kryssrutan för det obligatoriska objektet.":::

> [!NOTE]
> <span data-ttu-id="f8b8f-167">Varje erbjudande måste ha minst en plan som valts för att uppdateringen ska ske.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="f8b8f-168">Om du vill ta bort alla planer som är relaterade till ett erbjudande tar du bort hela erbjudandet (se nästa avsnitt).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="f8b8f-169">Ta bort erbjudanden</span><span class="sxs-lookup"><span data-stu-id="f8b8f-169">Delete offers</span></span>

<span data-ttu-id="f8b8f-170">På sidan Hantera Marketplace markerar du kryssrutan bredvid erbjudandets namn (se skärmen ovan) och väljer Ta **bort objekt.**</span><span class="sxs-lookup"><span data-stu-id="f8b8f-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="f8b8f-171">Aktivera/inaktivera privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f8b8f-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="f8b8f-172">På sidan Hantera Marketplace ser du någon av dessa banderoller, som visar det aktuella tillståndet för privat Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="f8b8f-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Visar banderollen &quot;Inaktivera tillstånd&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Visar banderollen &quot;Aktivera tillstånd&quot;.":::

<span data-ttu-id="f8b8f-175">Du kan aktivera eller inaktivera privata Azure Marketplace efter behov.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="f8b8f-176">Om den är inaktiverad **väljer du Aktivera privat Marketplace** för att aktivera.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="f8b8f-177">Om aktiverad väljer du **Inaktivera privat Marketplace för** att inaktivera.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="f8b8f-178">Meddelandecenter Azure Marketplace privata meddelanden</span><span class="sxs-lookup"><span data-stu-id="f8b8f-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="f8b8f-179">Meddelandecenter består av tre typer av meddelanden och låter Marketplace-administratören vidta åtgärder baserat på meddelandet:</span><span class="sxs-lookup"><span data-stu-id="f8b8f-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="f8b8f-180">Begäranden om godkännande från användare för objekt som inte finns i listan över godkända (se [Begäran om att lägga till erbjudanden eller planer](#request-to-add-offers-or-plans) nedan).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="f8b8f-181">Meddelanden om ny plan för erbjudanden som redan har en eller flera planer i listan över godkända.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="f8b8f-182">Planmeddelanden för objekt som finns i listan över godkända men som har tagits bort från den globala Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="f8b8f-183">Så här kommer du åt meddelandecentret:</span><span class="sxs-lookup"><span data-stu-id="f8b8f-183">To access the notification center:</span></span>

1. <span data-ttu-id="f8b8f-184">Välj **Meddelanden** på menyn till vänster.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="f8b8f-185">[![Visar menyn Meddelanden.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="f8b8f-186">Välj ellipsmenyn för fler åtgärder.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Visar resultat från menyn Fler alternativ.":::

1. <span data-ttu-id="f8b8f-188">För planbegäranden **öppnar Visa begäranden** formuläret för begäran om godkännande där du kan granska alla användarförfrågningar för det specifika erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="f8b8f-189">Välj **Godkänn** eller **Avvisa.**</span><span class="sxs-lookup"><span data-stu-id="f8b8f-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="f8b8f-190">[![Visar alternativen för att godkänna och avvisa.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="f8b8f-191">Välj den plan som ska godkännas från den nedrullningsna menyn.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="f8b8f-192">Lägg till en kommentar och välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="f8b8f-193">Bläddra bland privata Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f8b8f-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="f8b8f-194">När Privat Azure Marketplace aktiverats ser användarna vilka planer som Marketplace-administratören har godkänt.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="f8b8f-195">Ett grönt **meddelande om** godkänd anger ett partnererbjudande (inte Microsoft) som har godkänts.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="f8b8f-196">Ett blått **meddelande om** godkänd anger ett Microsoft-erbjudande (inklusive [godkända Linux-distributioner)](/azure/virtual-machines/linux/endorsed-distros)som har godkänts.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="f8b8f-197">Användare kan filtrera mellan erbjudanden som är och inte är godkända:</span><span class="sxs-lookup"><span data-stu-id="f8b8f-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="f8b8f-198">[![Visar filtreringsalternativet.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="f8b8f-199">Köp eller distribuera i privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f8b8f-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="f8b8f-200">Även om sidupplevelsen för produktinformation liknar den globala Azure Marketplace finns det tre privata Azure Marketplace specifika scenarier.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="f8b8f-201">När en användare väljer en godkänd plan **aktiveras** knappen Skapa:</span><span class="sxs-lookup"><span data-stu-id="f8b8f-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="f8b8f-202">[![Visar erbjudandebanderollen med information om att en plan kan skapas.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="f8b8f-203">Om ett produktplansval inte visas på produktinformationssidan men administratören har godkänt en eller  flera planer, visas en banderoll med information om vilka planer som har godkänts och knappen Skapa är aktiverad:</span><span class="sxs-lookup"><span data-stu-id="f8b8f-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="f8b8f-204">[![Visar erbjudandebanderollen med information om att en plan kan skapas och visar tillgängliga planer.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="f8b8f-205">När en användare väljer en icke-godkänd plan visas planen som inte godkänd i en banderoll och **knappen Skapa** inaktiveras.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="f8b8f-206">Användaren kan fortfarande begära att lägga till planen i listan över godkända (se nästa avsnitt).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="f8b8f-207">Begäran om att lägga till erbjudanden eller planer</span><span class="sxs-lookup"><span data-stu-id="f8b8f-207">Request to add offers or plans</span></span>

<span data-ttu-id="f8b8f-208">Du kan begära att lägga till ett offentligt erbjudande eller en plan som inte har godkänts i det privata Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="f8b8f-209">Välj **Begäran att lägga till i** banderollen för att öppna formuläret för **åtkomstbegäran.**</span><span class="sxs-lookup"><span data-stu-id="f8b8f-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="f8b8f-210">[![Visar banderollen med länken "Request to add" (Begäran om att lägga till).](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="f8b8f-211">[![Visar formuläret för åtkomstbegäran för erbjudanden eller planer.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="f8b8f-212">Välj vilka planer som ska läggas till i begäran ( Vilken **plan** som helst meddelar Marketplace-administratören att du inte har någon inställning för en plan i ett erbjudande).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="f8b8f-213">Lägg till **en motivering** och välj **Begäran** för att skicka din begäran.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="f8b8f-214">[![Visar formuläret för åtkomstbegäran för erbjudanden eller planer med exempelposter.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="f8b8f-215">En indikation för en väntande begäran visas i formuläret Åtkomstbegäran med alternativet **Begär begäran .**</span><span class="sxs-lookup"><span data-stu-id="f8b8f-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="f8b8f-216">[![Visar en lista över godkända eller väntande planer med länken Förfrågningsbegäran.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="f8b8f-217">När det har skickats skickas formuläret för begäran om godkännande till [Meddelandecenter](#private-azure-marketplace-notification-center) så att Marketplace-administratören kan granska begäran och vidta åtgärder.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="f8b8f-218">Godkännande till privat Marknadsplats anger inte anskaffning av en lösning.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="f8b8f-219">Vanliga frågor och svar</span><span class="sxs-lookup"><span data-stu-id="f8b8f-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="f8b8f-220">Jag blockerar redan Marketplace-program från tredje part via Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="f8b8f-221">Hur skiljer sig detta åt?</span><span class="sxs-lookup"><span data-stu-id="f8b8f-221">How is this different?</span></span>

<span data-ttu-id="f8b8f-222">Det finns för närvarande två sätt att begränsa tjänster från tredje part på Marketplace:</span><span class="sxs-lookup"><span data-stu-id="f8b8f-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="f8b8f-223">Via EA-portalen eller Azure Portal inaktiverar du tjänster från tredje part eller begränsar till "endast kostnadsfria SKU:er eller BYOL-SKU:er".</span><span class="sxs-lookup"><span data-stu-id="f8b8f-223">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Visar hur du begränsar tjänster i Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Visar hur du begränsar tjänster i E A-portalen.":::

2. <span data-ttu-id="f8b8f-226">Skapa en Azure-princip för att endast tillåta specifika virtuella datorer.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="f8b8f-227">Mer information om hur du tillämpar principer för virtuella Windows-datorer finns [i Tillämpa principer på virtuella Windows-datorer med Azure Resource Manager](/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="f8b8f-228">Privata Azure Marketplace ger mer flexibilitet när det gäller att begränsa och tillåta specifika erbjudanden och planer.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="f8b8f-229">Den informerar slutanvändarna om tillgängligheten för distribution i Marketplace-galleriet även innan de försöker distribuera tjänster från tredje part.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="f8b8f-230">Om du vill tillåta distribution av tjänster från tredje part anger du Azure Marketplace på På/Aktiverad i EA-portalen och Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="f8b8f-231">Privata Azure Marketplace kan hantera partnerlösningar som inte är begränsade till virtuella datorer.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="f8b8f-232">Privata Azure Marketplace kan väljas på plannivå och kan även ange "Aktuell och framtida plan".</span><span class="sxs-lookup"><span data-stu-id="f8b8f-232">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="f8b8f-233">Privata Azure Marketplace kan informera slutanvändarna direkt om vad som kan och inte kan distribueras.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="f8b8f-234">Vad är skillnaden mellan ett privat erbjudande och ett privat Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="f8b8f-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="f8b8f-235">Med **ett privat erbjudande** kan utgivare skapa planer som endast är synliga för målkunder.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="f8b8f-236">På så sätt kan de dela anpassade lösningar privat med förhandlad prissättning, privata villkor och specialiserade konfigurationer.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="f8b8f-237">Mer information finns i [Privata erbjudanden på den kommersiella marknadsplatsen.](/azure/marketplace/private-offers)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="f8b8f-238">**Privata Azure Marketplace** i Azure Portal administratörer i förväg godkänna vilka lösningar från tredje part som deras användare kan distribuera.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="f8b8f-239">Med en privat Azure Marketplace kan användarna dra nytta av fördelarna med Azure Marketplace genom att hitta, köpa och distribuera kompatibla erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="f8b8f-240">För att kunna hantera prenumerationsbaserade privata erbjudanden på privat Marketplace måste Marketplace-administratören minst ha rollen "läsa" för den specifika prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="f8b8f-241">Jag har lagt till ett privat erbjudande i Azure Marketplace, varför visas det inte på fliken Hantera Marketplace?</span><span class="sxs-lookup"><span data-stu-id="f8b8f-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="f8b8f-242">Prenumerationsbaserade privata erbjudanden visas bara för de angivna prenumerationerna i inställningarna för privat erbjudande.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="f8b8f-243">Om du vill visa det privata erbjudandet ser du till att det globala prenumerationsfiltret visar alla prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="f8b8f-244">[![Visar filtret för privat marknadsplats.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f8b8f-244">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="f8b8f-245">Kan vi inkludera anpassade avbildningar i privata Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="f8b8f-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="f8b8f-246">Nej.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-246">No.</span></span> <span data-ttu-id="f8b8f-247">Privata Azure Marketplace it-administratörer kan hantera och hantera lösningar från tredje part från globala Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="f8b8f-248">Eftersom anpassade avbildningar inte finns på globala Azure Marketplace kan IT-administratören inte välja dina anpassade avbildningar.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="f8b8f-249">Om du vill dela anpassade avbildningar använder du [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="f8b8f-250">Steg-för-steg-guide Skapa en Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="f8b8f-251">Skapa en avbildningsdefinition i en SIG.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="f8b8f-252">Kunden bör välja **Generaliserad** för fältet OS-tillstånd.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="f8b8f-253">([CLI,](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition) [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="f8b8f-254">Ta en hanterad avbildning till Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="f8b8f-255">SIG VM-avbildningarna skulle finnas i en prenumeration.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="f8b8f-256">Om du vill göra den tillgänglig för andra prenumerationer använder du en appregistrering ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="f8b8f-257">Varför visas vissa erbjudanden som **godkända som standard** även om utgivaren inte är Microsoft?</span><span class="sxs-lookup"><span data-stu-id="f8b8f-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="f8b8f-258">Microsoft har stöd för Linux och teknik med öppen källkod i Azure.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="f8b8f-259">[Godkända Linux-distributioner](/azure/virtual-machines/linux/endorsed-distros) stöds i Azure och priset är integrerat i virtuella datorer.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="f8b8f-260">Eftersom Azure Linux-agenten redan är förinstallerad på Azure Marketplace behandlas den som ett Microsoft-erbjudande.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="f8b8f-261">Eftersom Microsoft-erbjudanden godkänns som standard kan godkända Linux-distributioner inte hanteras i privata Azure Marketplace och godkänns som standard.</span><span class="sxs-lookup"><span data-stu-id="f8b8f-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="f8b8f-262">Kontakta supporten</span><span class="sxs-lookup"><span data-stu-id="f8b8f-262">Contact support</span></span>

- <span data-ttu-id="f8b8f-263">Om Azure Marketplace support kan du besöka [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="f8b8f-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>