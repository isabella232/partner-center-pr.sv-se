---
title: Skapa och hantera privat Azure Marketplace i Azure Portal
description: Lär dig mer om att skapa och hantera privata Azure Marketplace (för hands version) i Azure Portal.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: f62c9aef13b51ba2db42b267d7620f506bbdc1ec
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/21/2020
ms.locfileid: "95006947"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Skapa och hantera privat Azure Marketplace (för hands version) i Azure Portal

Med privat Azure Marketplace (för hands version) kan administratörer styra vilka lösningar från tredje part som användarna kan använda. Det gör det genom att låta dig distribuera endast erbjudanden som du godkänner och som uppfyller företagets principer. Med en privat Azure Marketplace kan användarna söka i onlinebutiken efter kompatibla erbjudanden för köp och distribution. 

Som Marketplace-administratör (tilldelad roll) börjar du med en inaktive rad och en tom privat lagrings plats där du kan lägga till godkända erbjudanden och planer. Den här artikeln beskriver hur du skapar, hanterar och aktiverar privat Azure Marketplace för dina användare.

Obs!

- En privat Azure Marketplace finns på klient nivå, så alla användare under klienten ser samma granskade lista.
- Alla Microsoft-lösningar läggs automatiskt till i privata Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Tilldela rollen Marketplace-administratör

Den globala klient organisationen måste tilldela rollen **Marketplace-administratör** till den privata Azure Marketplace-administratören som ska hantera den privata lagringen.

>[!IMPORTANT]
> Åtkomst till privat Azure Marketplace-hantering är bara tillgänglig för IT-administratörer med rollen Marketplace-administratör tilldelad.

### <a name="prerequisites"></a>Förutsättningar

Du måste uppfylla dessa krav innan du kan tilldela rollen Marketplace-administratör till en användare i klient omfånget:

- Du har åtkomst till en **Global administratörs** användare.
- Klienten har minst en prenumeration (kan vara av valfri typ).
- Den globala administratörs användaren tilldelas rollen **deltagare** eller högre för den valda prenumerationen.
- Den globala administratörs användaren har förhöjd åtkomst inställt på **Ja** (se [öka åtkomsten för att hantera alla Azure-prenumerationer och hanterings grupper](/azure/role-based-access-control/elevate-access-global-admin)).

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Tilldela rollen Marketplace-administratör med PowerShell

Använd följande PowerShell-skript för att tilldela rollen Marketplace-administratör; den kräver följande parametrar:

- **TenantId:** ID: t för klient organisationen i omfånget (Marketplace admin-rollen kan tilldelas i klientens omfång).
- **SubscriptionId:** En prenumeration som den globala administratören har rollen **deltagare** eller högre tilldelad.
- **GlobalAdminUsername:** Användar namnet för den globala administratören.
- **UsernameToAssignRoleFor:** Det användar namn som Marketplace-administratörskonsolen ska tilldelas till.

> [!NOTE]
> För gäst användare som har bjudits in till klienten kan det ta upp till 48 timmar tills deras konto är tillgängligt för att tilldela Marketplace-administratörskonsolen. Mer information finns i [Egenskaper för en Azure Active Directory B2B-samarbets användare](/azure/active-directory/b2b/user-properties).

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

Mer information om de cmdletar som finns i AZ. Portal PowerShell-modulen finns [Microsoft Azure PowerShell: portalens instrument panels-cmdletar](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Skapa en privat Azure Marketplace

1. Logga in på [Azure-portalen](https://portal.azure.com/).
2. Välj **alla tjänster** och sedan **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal huvud fönstret.":::

3. Välj **privat Marketplace** från alternativen till vänster.

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Välja Privat Marketplace i Azure Portal huvud fönstret.":::

4. Välj **Kom igång** för att skapa en privat Azure Marketplace (du behöver bara göra det här en gång).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Välj kom igång i Azure Portal huvud fönstret.":::

    Om den privata Azure Marketplace redan finns för den här klienten, är **Hantera Marketplace** valt som standard.

5. När du är klar har du en tom och inaktive rad privat Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Den tomma privata Azure Marketplace-skärmen.":::

## <a name="add-items-from-gallery"></a>Lägg till objekt från galleriet

Ett objekt är en kombination av ett erbjudande och en plan. Du kan söka efter och lägga till objekt på sidan Hantera Marketplace.

1. Välj **Lägg till objekt**.

2. Bläddra i **galleriet** eller Använd Sök fältet för att hitta det objekt som du vill använda.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Bläddra i galleriet eller Använd Sök fältet.":::

3. Som standard kommer alla aktuella planer att läggas till i listan över tillåtna när du lägger till ett nytt erbjudande. Om du vill ändra plan urvalet innan du lägger till de valda objekten väljer du den nedrullningsbara menyn i erbjudande panelen och uppdaterar de nödvändiga planerna.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Uppdatera nödvändiga planer.":::

4. Välj **klar** längst ned till vänster när du har gjort dina val.

>[!Note]
> **Lägg till objekt** till Marketplace kommer endast att vara tillgängligt för erbjudanden som inte kommer från Microsoft. Microsoft-erbjudanden tillåts som standard.

## <a name="edit-item-plans"></a>Redigera artikel planer

Du kan redigera ett objekts planer på sidan Hantera Marketplace.

1. I kolumnen **planer** granskar du de tillgängliga planerna från List menyn för det objektet.
2. Markera eller avmarkera kryss rutorna för att välja vilka planer som ska vara tillgängliga för dina användare.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Markera eller avmarkera kryss rutan för det begärda objektet.":::

> [!NOTE]
> Varje erbjudande måste ha minst en plan vald för att uppdateringen ska ske. Ta bort alla planer som är relaterade till ett erbjudande genom att ta bort hela erbjudandet (se nästa avsnitt).

## <a name="delete-offers"></a>Ta bort erbjudanden

På sidan Hantera marknads plats markerar du kryss rutan bredvid namnet på erbjudandet (se skärmen ovan) och väljer **ta bort objekt**.

## <a name="enabledisable-private-azure-marketplace"></a>Aktivera/inaktivera privat Azure Marketplace

På sidan Hantera Marketplace visas en av dessa banderoller som visar det aktuella läget för privat Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Inaktivera State-banderoll":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Aktivera State-banderoll":::

Du kan aktivera eller inaktivera privat Azure Marketplace efter behov.

1. Om det är inaktiverat väljer du **aktivera privat Marketplace** för att aktivera.
2. Om aktive rad väljer du **Inaktivera privat Marketplace** för att inaktivera.

## <a name="browsing-private-azure-marketplace"></a>Bläddra i privat Azure Marketplace

När privat Azure Marketplace är aktiverat ser användarna vilka planer som Marketplace-administratören har tillåtit.

- Ett grönt **tillåtet** meddelande anger ett erbjudande för partner (inte Microsoft) som är tillåtet.
- Ett blått **tillåtet** meddelande indikerar ett Microsoft-erbjudande som är tillåtet.

Användare kan filtrera mellan erbjudanden som är och inte tillåtna:

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Filtrerings alternativ.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Köp eller distribuera i privat Azure Marketplace

Även om produkt informationens sid upplevelse liknar den offentliga Azure Marketplace finns det tre privata Azure Marketplace-scenarier.

- När en användare väljer en tillåten plan aktive ras knappen **skapa** :

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Erbjudande banderoll med en plan kan skapas.":::

- När en användare väljer en icke-tillåten plan, visar en banderoll om att planen inte är tillåten och knappen **skapa** är inaktive rad.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Erbjudande banderollen det går inte att skapa en plan.":::

- Om ett val av produkt plan inte visas på sidan produkt information men administratören har godkänt en eller flera planer, visar en banderoll vilka planer som är tillåtna och knappen **skapa** är aktive rad:

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Erbjudande banderoll som visar att en plan kan skapas och visar tillgängliga planer.":::

## <a name="contact-support"></a>Kontakta supporten

Besök [Microsoft Q&A](/answers/products/)för support för Azure Marketplace. 
