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
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Skapa och hantera privata Azure Marketplace i Azure Portal

Privata Azure Marketplace låter administratörer styra vilka lösningar från tredje part som användarna kan använda. Det gör det genom att låta användaren bara distribuera erbjudanden som godkänts av administratören och följa företagets principer. Med privat Azure Marketplace kan användarna söka i onlinebutiken efter kompatibla erbjudanden för köp och distribution.

Som Marketplace-administratör (tilldelad roll) börjar du med en inaktive rad och en tom privat lagrings plats där du kan lägga till godkända erbjudanden och planer. Den här artikeln beskriver hur du tilldelar den roll som krävs, skapar ett privat lager, hanterar objekt, godkänner användar förfrågningar och aktiverar privat Azure Marketplace för dina användare.

> [!NOTE]
> - En privat Azure Marketplace finns på klient nivå, så alla användare under klienten ser samma granskade lista.
> - Alla Microsoft-lösningar (inklusive godkända [Linux-distributioner](/azure/virtual-machines/linux/endorsed-distros)) läggs automatiskt till i privata Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Tilldela rollen Marketplace-administratör

Den globala klient organisationen måste tilldela rollen **Marketplace-administratör** till den privata Azure Marketplace-administratören som ska hantera den privata lagringen.

>[!IMPORTANT]
> Åtkomst till privat Azure Marketplace-hantering är bara tillgänglig för IT-administratörer med rollen Marketplace-administratör tilldelad.

### <a name="prerequisites"></a>Förutsättningar

Dessa krav måste vara uppfyllda innan du kan tilldela rollen Marketplace-administratör till en användare i klient omfånget:

- Du har åtkomst till en **Global administratörs** användare.
- Klienten har minst en prenumeration (kan vara av valfri typ).
- Den globala administratörs användaren tilldelas rollen **deltagare** eller högre för den valda prenumerationen.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Tilldela rollen Marketplace-administratör med åtkomst kontroll (IAM)

1. Logga in på [Azure-portalen](https://portal.azure.com/).
1. Välj **alla tjänster** och sedan **Marketplace**.
1. Välj **privat Marketplace** på menyn till vänster.

    [![Visar meny alternativet privat Marketplace på vänster sida av Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. Välj **åtkomst kontroll (IAM)** för att tilldela rollen Marketplace-administratör.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Visar skärmen I A M-åtkomst kontroll.":::

1. Välj **+ Lägg till** > **Lägg till rolltilldelning**.
1. Välj **Marketplace-administratör** under **roll**.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Visar menyn roll tilldelning.":::

1. Välj önskad användare i list rutan och välj sedan **Slutför**.

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

Mer information om de cmdletar som finns i AZ. Portal PowerShell-modulen finns [Microsoft Azure PowerShell: portalens instrument panels-cmdletar](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Skapa en privat Azure Marketplace

1. Logga in på [Azure-portalen](https://portal.azure.com/).
2. Välj **alla tjänster** och sedan **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Visar Azure Portal huvud fönstret.":::

3. Välj **privat Marketplace** på menyn till vänster.

4. Välj **Kom igång** för att skapa en privat Azure Marketplace (du behöver bara göra det här en gång).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Visar hur du väljer huvud fönstret kom igång i Azure Portal.":::

    Om den privata Azure Marketplace redan finns för den här klienten, är **Hantera Marketplace** valt som standard.

5. När du är klar har du en tom och inaktive rad privat Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Visar den tomma privata Azure Marketplace-skärmen.":::

## <a name="add-items-from-gallery"></a>Lägg till objekt från galleriet

Ett objekt är en kombination av ett erbjudande och en plan. Du kan söka efter och lägga till objekt på sidan Hantera Marketplace.

1. Välj **Lägg till objekt**.

2. Bläddra i **galleriet** eller Använd Sök fältet för att hitta det objekt som du vill använda.

    [![Visar hur du bläddrar i galleriet eller använder Sök fältet.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. Som standard kommer alla aktuella planer att läggas till i listan över godkända när du lägger till ett nytt erbjudande. Om du vill ändra plan urvalet innan du lägger till de valda objekten väljer du den nedrullningsbara menyn i erbjudande panelen och uppdaterar de nödvändiga planerna.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Visar hur du uppdaterar nödvändiga planer.":::

4. Välj **klar** längst ned till vänster när du har gjort dina val.

>[!Note]
> **Lägg till objekt** till Marketplace kommer endast att vara tillgängligt för erbjudanden som inte kommer från Microsoft. Microsoft-lösningar (inklusive godkända [Linux-distributioner](/azure/virtual-machines/linux/endorsed-distros)) märks som "godkända som standard" och kan inte hanteras i privat Marketplace.

## <a name="edit-items-plans"></a>Redigera objektets planer

Du kan redigera ett objekts planer på sidan Hantera Marketplace.

1. I kolumnen **planer** granskar du de tillgängliga planerna från List menyn för det objektet.
2. Markera eller avmarkera kryss rutorna för att välja vilka planer som ska vara tillgängliga för dina användare.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Visar hur du markerar eller avmarkerar kryss rutan för det begärda objektet.":::

> [!NOTE]
> Varje erbjudande måste ha minst en plan som valts för att uppdateringen ska ske. Ta bort alla planer som är relaterade till ett erbjudande genom att ta bort hela erbjudandet (se nästa avsnitt).

## <a name="delete-offers"></a>Ta bort erbjudanden

På sidan Hantera marknads plats markerar du kryss rutan bredvid namnet på erbjudandet (se skärmen ovan) och väljer **ta bort objekt**.

## <a name="enabledisable-private-azure-marketplace"></a>Aktivera/inaktivera privat Azure Marketplace

På sidan Hantera Marketplace visas en av dessa banderoller som visar det aktuella läget för privat Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Visar banderollen &quot;inaktivera tillstånd&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Visar banderollen Enable State.":::

Du kan aktivera eller inaktivera privat Azure Marketplace efter behov.

- Om det är inaktiverat väljer du **aktivera privat Marketplace** för att aktivera.
- Om aktive rad väljer du **Inaktivera privat Marketplace** för att inaktivera.

## <a name="private-azure-marketplace-notification-center"></a>Privat meddelande Center för Azure Marketplace

Notification Center består av tre typer av meddelanden och gör att Marketplace-administratören kan vidta åtgärder baserat på aviseringen:

- Godkännande begär Anden från användare för objekt som inte finns med i listan över godkända (se [begäran om att lägga till erbjudanden eller planer](#request-to-add-offers-or-plans) nedan).
- Nya plan meddelanden för erbjudanden som redan har en eller flera planer i listan över godkända.
- Tog bort plan meddelanden för objekt som finns i den godkända listan men som har tagits bort från den globala Azure Marketplace.

För att komma åt meddelande centret:

1. Välj **meddelanden** på menyn på den vänstra sidan.

    [![Visar menyn meddelanden.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. Välj menyn med tre punkter för fler åtgärder.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Visar meny resultatet fler alternativ.":::

1. För begäran om att **Visa förfrågningar** öppnar formuläret begäran om godkännande där du kan granska alla användar förfrågningar för det aktuella erbjudandet.
1. Välj **Godkänn** eller **avvisa**.

    [![Visar alternativen Godkänn och avvisa.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. Välj den plan som du vill godkänna på den nedrullningsbara menyn.
1. Lägg till en kommentar och välj **Skicka**.

## <a name="browsing-private-azure-marketplace"></a>Bläddra i privat Azure Marketplace

När privat Azure Marketplace är aktiverat ser användarna vilka planer som Marketplace-administratören har godkänt.

- Ett grönt **godkänt** meddelande anger ett erbjudande för partner (inte Microsoft) som är godkänt.
- Ett blått **godkänt** meddelande anger ett Microsoft-erbjudande (inklusive godkända [Linux-distributioner](/azure/virtual-machines/linux/endorsed-distros)) som är godkänt.

Användare kan filtrera mellan erbjudanden som är och inte är godkända:

[![Visar filtrerings alternativet.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Köp eller distribuera i privat Azure Marketplace

Även om produkt informationens sid upplevelse liknar den globala Azure Marketplace finns det tre privata Azure Marketplace-olika scenarier.

- När en användare väljer en godkänd plan aktive ras knappen **skapa** :

    [![Visar en banderoll för erbjudandet om att en plan kan skapas.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- Om ett val av produkt plan inte visas på sidan produkt information men administratören har godkänt en eller flera planer, visar en banderoll vilka planer som godkänns och knappen **skapa** är aktive rad:

    [![Visar banderollen erbjudande om att en plan kan skapas och Visa tillgängliga planer.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- När en användare väljer en icke godkänd plan, visar en banderoll om planen är inte godkänd och knappen **skapa** är inaktive rad. Användaren kan fortfarande begära att lägga till planen i den godkända listan (se nästa avsnitt).

## <a name="request-to-add-offers-or-plans"></a>Begäran om att lägga till erbjudanden eller planer

Du kan begära att lägga till ett offentligt erbjudande eller en plan som inte är godkänd i den privata Azure Marketplace.

1. Välj **begär att lägga till** i banderollen för att öppna **formuläret** åtkomstbegäran.

    [![Visar banderollen med länken "begär att lägga till".](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![Visar formuläret för åtkomstbegäran för erbjudanden eller planer.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. Välj vilka planer som ska läggas till i begäran (**alla planer** meddelar Marketplace-administratören att du inte har någon preferens för en prenumeration i ett erbjudande).

1. Lägg till en **motivering** och välj **begäran** för att skicka in din begäran.
  
    [![Visar formuläret för åtkomstbegäran för erbjudanden eller planer med exempel poster.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. En indikation för en väntande begäran visas i formuläret åtkomstbegäran med ett alternativ för att **återkalla begäran**.

    [![Visar en lista över godkända eller väntande planer med länken återkalla begäran.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> När den har skickats skickas formuläret för godkännande förfrågning till [meddelande centret](#private-azure-marketplace-notification-center) för Marketplace-administratören för att granska begäran och vidta åtgärder.

## <a name="frequently-asked-questions-faqs"></a>Vanliga frågor och svar

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Jag blockerar redan Marketplace-program från tredje part via Azure Policy. Hur skiljer sig detta?

Det finns för närvarande två sätt att begränsa tjänster från tredje part på Marketplace:

1. I EA-portalen eller Azure Portal inaktiverar du tjänster från tredje part eller begränsar till "kostnads fri eller BYOL SKU: er".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Visar hur du begränsar tjänster i Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Visar hur du begränsar tjänster i E-portalen.":::

2. Skapa en Azure-princip för att bara tillåta vissa virtuella datorer. Mer information om hur du tillämpar principer för virtuella Windows-datorer finns i [tillämpa principer på virtuella Windows-datorer med Azure Resource Manager](/azure/virtual-machines/windows/policy).

Privata Azure Marketplace ger större flexibilitet när det gäller att begränsa och tillåta vissa erbjudanden och planer. Det informerar slutanvändarna om tillgänglighet för distribution i Marketplace-galleriet även innan de försöker distribuera tjänster från tredje part. Om du vill tillåta distribution av tjänster från tredje part ställer du in Azure Marketplace till på/aktiverat i EA-portalen och Azure Portal.

- Privata Azure Marketplace kan granska partner lösningar som inte är begränsade till virtuella datorer.
- Privata Azure Marketplace kan granska på plannivå och kan också ange "nuvarande och framtida plan".
- Privata Azure Marketplace kan informera slutanvändarna om vad som kan och inte kan distribueras.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Vad är skillnaden mellan ett privat erbjudande och en privat Azure Marketplace?

Med ett **privat erbjudande** kan utgivare skapa planer som endast är synliga för riktade kunder. Detta gör det möjligt för dem att dela anpassade lösningar med förhandlad prissättning, privata villkor och specialiserade konfigurationer. Mer information finns [i privata erbjudanden på den kommersiella marknaden](/azure/marketplace/private-offers).

Med den **privata Azure Marketplace** i Azure Portal kan administratörer godkänna vilka lösningar från tredje part som användarna kan distribuera. Med en privat Azure Marketplace kan användarna dra nytta av fördelarna med Azure Marketplace genom att söka efter, köpa och distribuera kompatibla erbjudanden. För att hantera prenumerations privata erbjudanden i privat Marketplace måste Marketplace-administratören ha minst "Läs"-rollen för den aktuella prenumerationen.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Jag har lagt till ett privat erbjudande på den privata Azure Marketplace, varför visas det inte på fliken Hantera Marketplace?

Prenumerations privata erbjudanden visas bara för de listade prenumerationerna i inställningarna för privata erbjudanden. Om du vill visa det privata erbjudandet ser du till att det globala prenumerations filtret visar alla prenumerationer.

[![Visar filtret för privata marknads platser.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Kan vi inkludera anpassade bilder i privata Azure Marketplace?

Nej. Med privata Azure Marketplace kan IT-administratörer hantera och granska lösningar från tredje part från globala Azure Marketplace. Eftersom anpassade avbildningar inte finns på globala Azure Marketplace kan IT-administratören inte välja och välja anpassade avbildningar. Använd [delat avbildnings Galleri](/azure/virtual-machines/shared-image-galleries)om du vill dela anpassade avbildningar.

1. Steg-för-steg-guide skapa ett delat bild galleri (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).
2. Skapa en avbildnings definition i en SIG. Kunden bör välja **generaliserad** för fältet OS-tillstånd. ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Placera hanterade avbildningar i det delade bild galleriet ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. Avbildningarna för SIG-VM finns i en prenumeration. Använd en app-registrering ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)) för att göra det tillgängligt för andra prenumerationer.

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Varför visas vissa erbjudanden som har **godkänts som standard** även om utgivaren inte är Microsoft?

Microsoft stöder Linux och teknik med öppen källkod i Azure. Godkända [Linux-distributioner](/azure/virtual-machines/linux/endorsed-distros) stöds i Azure och priset är integrerat i virtuella datorer. Eftersom Azure Linux-agenten redan är förinstallerad på Azure Marketplace, behandlas det som ett Microsoft-erbjudande. Eftersom Microsoft-erbjudanden har godkänts som standard kan inte godkända Linux-distributioner hanteras i privata Azure Marketplace och godkänns som standard.

## <a name="contact-support"></a>Kontakta supporten

- Besök [Microsoft Q&A](/answers/products/)för support för Azure Marketplace.