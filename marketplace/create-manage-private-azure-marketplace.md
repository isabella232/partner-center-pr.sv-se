---
title: Skapa och hantera privata Azure Marketplace i Azure Portal
description: Lär dig mer om att skapa och hantera Azure Marketplace (förhandsversion) i Azure Portal i den äldre vyn. Med Azure Marketplace (förhandsversion) kan administratörer styra vilka tredjepartslösningar deras användare kan använda.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 08/10/2021
ms.openlocfilehash: da44807519f18d6aa17e41d8e81b9ad774e40d2d
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246678"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Skapa och hantera privata Azure Marketplace i Azure Portal

> [!NOTE]
> Den här artikeln beskriver äldre privata Azure Marketplace. Den nya vyn Samlingar finns i den här [nya artikeln i](create-manage-private-azure-marketplace-new.md) stället.

Privata Azure Marketplace administratörer styra vilka lösningar från tredje part deras användare kan använda. Den gör detta genom att tillåta användaren att endast distribuera erbjudanden som har godkänts av administratören och som uppfyller företagets principer. Med Private Azure Marketplace kan användarna söka i onlinebutiken efter kompatibla erbjudanden att köpa och distribuera.

Som Marketplace-administratör (tilldelad roll) börjar du med ett inaktiverat och tomt privat arkiv där du kan lägga till godkända erbjudanden och planer. Den här artikeln förklarar hur du tilldelar den roll som krävs, skapar ett privat arkiv, hanterar objekt, godkänner användarbegäranden och aktiverar privata Azure Marketplace för dina användare.

> [!NOTE]
> - Privata Azure Marketplace på klientorganisationsnivå, så alla användare under klientorganisationen ser samma curated lista.
> - Alla Microsoft-lösningar (inklusive [godkända Linux-distributioner)](/azure/virtual-machines/linux/endorsed-distros)läggs automatiskt till i privata Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Tilldela administratörsrollen för Marketplace

Klientorganisationens Global administratör tilldela **Administratörsrollen för Marketplace** till den privata Azure Marketplace som ska hantera det privata arkivet.

>[!IMPORTANT]
> Åtkomst till privat Azure Marketplace är endast tillgänglig för IT-administratörer med administratörsrollen Marketplace tilldelad.

### <a name="prerequisites"></a>Förutsättningar

Dessa krav måste vara uppfyllda innan du kan tilldela administratörsrollen för Marketplace till en användare i klientorganisationsomfånget:

- Du har åtkomst till en **Global administratör** användare.
- Klienten har minst en prenumeration (kan vara vilken typ som helst).
- Användaren Global administratör tilldelas rollen **Deltagare eller** högre för den valda prenumerationen.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Tilldela administratörsrollen för Marketplace med åtkomstkontroll (IAM)

1. Logga in på [Azure-portalen](https://portal.azure.com/).

1. Välj **Alla tjänster** och sedan **Marketplace**.

1. Välj **Privat Marketplace** på menyn till vänster.

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Visar menyalternativet privat marketplace till vänster på Marketplace.":::

1. Välj **Åtkomstkontroll (IAM) för** att tilldela administratörsrollen för Marketplace.

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Visar skärmen IA M-åtkomstkontroll.":::

1. Välj **+ Lägg till** > **Lägg till rolltilldelning**.

1. Under **Roll** väljer du **Marketplace-administratör.**

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Visar menyn Rolltilldelning.":::

1. Välj önskad användare i listrutan och välj sedan **Klar.**

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Tilldela administratörsrollen för Marketplace med PowerShell

Använd följande PowerShell-skript för att tilldela administratörsrollen för Marketplace: Det kräver följande parametrar:

- **TenantId:** ID:t för klienten i omfånget (Marketplace-administratörsrollen kan tilldelas i klientorganisationsomfånget).
- **SubscriptionId:** En prenumeration som den globala administratören har rollen **Deltagare eller** högre tilldelad.
- **GlobalAdminUsername:** Användarnamnet för den globala administratören.
- **UsernameToAssignRoleFor:** Användarnamnet som administratörsrollen för Marketplace ska tilldelas.

> [!NOTE]
> För gästanvändare som bjudits in till klientorganisationen kan det ta upp till 48 timmar innan deras konto är tillgängligt för tilldelning av rollen Marketplace-administratör. Mer information finns i Egenskaper [för en Azure Active Directory B2B-samarbetsanvändare](/azure/active-directory/b2b/user-properties).

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

Mer information om cmdletarna i PowerShell-modulen Az.Portal finns i [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Skapa privat Azure Marketplace

1. Logga in på [Azure-portalen](https://portal.azure.com/).
2. Välj **Alla tjänster** och sedan **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Visar Azure Portal huvudfönstret.":::

3. Välj **Privat Marketplace** på menyn till vänster.

4. Välj **Kom igång** att skapa privata Azure Marketplace (du behöver bara göra detta en gång).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Visar hur du väljer &quot;Kom igång på Azure Portal&quot;-huvudfönstret.":::

    Om privat Azure Marketplace redan finns för den här klientorganisationen väljs Hantera **Marketplace** som standard.

5. När det är klart har du en tom och inaktiverad privat Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Visar den tomma privata Azure Marketplace skärmen.":::

## <a name="add-items-from-gallery"></a>Lägga till objekt från galleriet

Ett objekt är en kombination av ett erbjudande och en plan. Du kan söka efter och lägga till objekt på sidan Hantera Marketplace.

1. Välj **Lägg till objekt.**

2. Bläddra i **galleriet** eller använd sökfältet för att hitta det objekt som du vill använda.

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Visar hur du bläddrar i galleriet eller använder sökfältet.":::

3. När du lägger till ett nytt erbjudande läggs som standard alla aktuella planer till i listan över godkända planer. Om du vill ändra valet av plan innan du lägger till de valda objekten väljer du den nedrullningsna menyn i erbjudandets panel och uppdaterar de planer som krävs.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Visar hur du uppdaterar de planer som krävs.":::

4. Välj **Klar** längst ned till vänster när du har gjort dina val.

>[!Note]
> **Lägg till** objekt på Marketplace kommer endast att vara tillgängligt för erbjudanden som inte kommer från Microsoft. Microsoft-lösningar [(inklusive godkända Linux-distributioner)](/azure/virtual-machines/linux/endorsed-distros)taggas som "Godkända som standard" och kan inte hanteras på privat Marketplace.

## <a name="edit-items-plans"></a>Redigera objektplaner

Du kan redigera ett objekts planer på sidan Hantera Marketplace.

1. Granska de **tillgängliga** planerna i den nedrullningsbara menyn för objektet i kolumnen Planer.

2. Markera eller avmarkera kryssrutorna för att välja vilka planer som ska göras tillgängliga för användarna.

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Visar hur du markerar eller avmarkerar kryssrutan för det obligatoriska objektet.":::

   > [!NOTE]
   > Varje erbjudande måste ha minst en plan som valts för att uppdateringen ska ske. Om du vill ta bort alla planer som är relaterade till ett erbjudande tar du bort hela erbjudandet (se nästa avsnitt).

## <a name="delete-offers"></a>Ta bort erbjudanden

På sidan Hantera Marketplace markerar du kryssrutan bredvid erbjudandets namn (se skärmen ovan) och väljer Ta **bort objekt.**

## <a name="enabledisable-private-azure-marketplace"></a>Aktivera/inaktivera privat Azure Marketplace

På sidan Hantera Marketplace ser du någon av dessa banderoller, som visar det aktuella tillståndet för privat Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Visar banderollen &quot;Inaktivera tillstånd&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Visar banderollen &quot;Aktivera tillstånd&quot;.":::

Du kan aktivera eller inaktivera privata Azure Marketplace efter behov.

- Om den är inaktiverad **väljer du Aktivera privat Marketplace** för att aktivera.
- Om aktiverad väljer du **Inaktivera privat Marketplace för** att inaktivera.

## <a name="private-azure-marketplace-notification-center"></a>Meddelandecenter Azure Marketplace privata meddelanden

Meddelandecenter består av tre typer av meddelanden och låter Marketplace-administratören vidta åtgärder baserat på meddelandet:

- Begäranden om godkännande från användare för objekt som inte finns i listan över godkända (se [Begäran om att lägga till erbjudanden eller planer](#request-to-add-offers-or-plans) nedan).
- Meddelanden om ny plan för erbjudanden som redan har en eller flera planer i listan över godkända.
- Planmeddelanden för objekt som finns i listan över godkända men som har tagits bort från den globala Azure Marketplace.

Så här kommer du åt meddelandecentret:

1. Välj **Meddelanden** på menyn till vänster.

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Visar menyn Meddelanden.":::

1. Välj ellipsmenyn för fler åtgärder.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Visar resultat från menyn Fler alternativ.":::

1. För planbegäranden **öppnar Visa begäranden** formuläret för begäran om godkännande där du kan granska alla användarförfrågningar för det specifika erbjudandet.
1. Välj **Godkänn** eller **Avvisa.**

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Visar alternativen för att godkänna och avvisa.":::

1. Välj den plan som ska godkännas från den nedrullningsna menyn.
1. Lägg till en kommentar och välj **Skicka**.

## <a name="browsing-private-azure-marketplace"></a>Bläddra bland privata Azure Marketplace

När Private Azure Marketplace har aktiverats ser användarna vilka planer som Marketplace-administratören har godkänt.

- Ett grönt **meddelande om** godkänd anger ett partnererbjudande (inte Microsoft) som har godkänts.
- Ett blått **meddelande om** godkänd anger ett Microsoft-erbjudande (inklusive [godkända Linux-distributioner)](/azure/virtual-machines/linux/endorsed-distros)som har godkänts.

Användare kan filtrera mellan erbjudanden som är och inte är godkända:

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Visar filtreringsalternativet.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Köpa eller distribuera i privat Azure Marketplace

Även om upplevelsen på produktinformationssidan liknar den globala Azure Marketplace finns det tre privata Azure Marketplace specifika scenarier.

- När en användare väljer en godkänd plan **aktiveras** knappen Skapa:

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Visar erbjudandebanderollen som visar att en plan kan skapas.":::

- Om ett val av produktplan inte visas på produktinformationssidan men administratören har godkänt en  eller flera planer, visas en banderoll med information om vilka planer som har godkänts och knappen Skapa är aktiverad:

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Visar erbjudandebanderollen som anger att en plan kan skapas och visar tillgängliga planer.":::

- När en användare väljer en icke-godkänd plan visas planen som inte godkänd i en banderoll och **knappen Skapa** inaktiveras. Användaren kan fortfarande begära att planen ska läggas till i listan över godkända (se nästa avsnitt).

## <a name="request-to-add-offers-or-plans"></a>Begäran om att lägga till erbjudanden eller planer

Du kan begära att lägga till ett offentligt erbjudande eller en plan som för närvarande inte är godkänd i privat Azure Marketplace.

1. Välj **Begäran att lägga till** i banderollen för att öppna formuläret för **åtkomstbegäran.**

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Visar banderollen med länken &quot;Begäran om att lägga till&quot;.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Visar formuläret för åtkomstbegäran för erbjudanden eller planer.":::

1. Välj vilka planer som ska läggas till i begäran ( Alla **planer** talar om för Marketplace-administratören att du inte har någon inställning för en plan i ett erbjudande).

1. Lägg till **en motivering** och välj **Begäran** för att skicka din begäran.

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Visar formuläret för åtkomstbegäran för erbjudanden eller planer med exempelposter.":::

1. En indikation för en väntande begäran visas i formuläret Åtkomstbegäran med alternativet **Begär begäran**.

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Visar en lista över godkända eller väntande planer med länken Förfrågningsbegäran.":::

> [!NOTE]
> När formuläret för begäran om godkännande har skickats skickas det till [Meddelandecenter](#private-azure-marketplace-notification-center) så att Marketplace-administratören kan granska begäran och vidta åtgärder.

> [!CAUTION]
> Godkännande till privat Marketplace anger inte anskaffning av en lösning.

## <a name="frequently-asked-questions-faqs"></a>Vanliga frågor och svar

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Jag blockerar redan Marketplace-program från tredje part via Azure Policy. Hur är detta annorlunda?

Det finns för närvarande två sätt att begränsa tjänster från tredje part på Marketplace:

1. Via EA-portalen eller Azure Portal inaktivera tjänster från tredje part eller begränsa till "endast kostnadsfria eller BYOL SKU:er".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Visar hur du begränsar tjänster i Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Visar hur du begränsar tjänster i E A-portalen.":::

2. Skapa en Azure-princip för att endast tillåta specifika virtuella datorer. Mer information om hur du tillämpar en princip för Windows virtuella datorer finns i Tillämpa principer på [Windows virtuella datorer med Azure Resource Manager](/azure/virtual-machines/windows/policy).

Privata Azure Marketplace ger större flexibilitet när det gäller att begränsa och tillåta specifika erbjudanden och planer. Den informerar slutanvändarna om tillgängligheten för distribution i Marketplace-galleriet även innan de försöker distribuera tjänster från tredje part. Om du vill tillåta distribution av tjänster från tredje part Azure Marketplace till På/Aktiverad i EA-portalen och Azure Portal.

- Privata Azure Marketplace kan hantera partnerlösningar som inte är begränsade till virtuella datorer.
- Privata Azure Marketplace kan väljas på plannivå och kan även ange "Aktuell och framtida plan".
- Privata Azure Marketplace kan informera slutanvändarna direkt om vad som kan och inte kan distribueras.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Vad är skillnaden mellan ett privat erbjudande och ett privat Azure Marketplace?

Med **ett privat erbjudande** kan utgivare skapa planer som endast är synliga för målkunder. På så sätt kan de privat dela anpassade lösningar med förhandlad prissättning, privata villkor och specialiserade konfigurationer. Mer information finns i [Privata erbjudanden på den kommersiella marknadsplatsen.](/azure/marketplace/private-offers)

**Privata Azure Marketplace** i Azure Portal administratörer förhandsbekänna vilka lösningar från tredje part som deras användare kan distribuera. Med en privat Azure Marketplace kan användarna dra nytta av fördelarna med Azure Marketplace genom att hitta, köpa och distribuera kompatibla erbjudanden. För att hantera prenumerationsbaserade privata erbjudanden på privat Marketplace måste Marketplace-administratören ha minst rollen "läsa" för den specifika prenumerationen.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Jag har lagt till ett privat erbjudande i Azure Marketplace, varför visas det inte på fliken Hantera Marketplace?

Prenumerationsbaserade privata erbjudanden visas bara för de angivna prenumerationerna i inställningarna för privat erbjudande. Om du vill visa det privata erbjudandet ser du till att det globala prenumerationsfiltret visar alla prenumerationer.

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Visar filtret för privat marknadsplats.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Kan vi inkludera anpassade avbildningar i privata Azure Marketplace?

Nej. Privata Azure Marketplace it-administratörer kan hantera och hantera lösningar från tredje part från globala Azure Marketplace. Eftersom anpassade avbildningar inte finns på Azure Marketplace kan IT-administratören inte välja dina anpassade avbildningar. Om du vill dela anpassade avbildningar använder du [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).

1. Steg-för-steg-guide Skapa en Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).
2. Skapa en avbildningsdefinition i en SIG. Kunden bör välja **Generaliserad** för fältet OS-tillstånd. ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Ta en hanterad avbildning Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. SIG VM-avbildningarna skulle finnas i en prenumeration. Om du vill göra den tillgänglig för andra prenumerationer använder du en appregistrering ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Varför visas vissa erbjudanden godkända **som standard även** om utgivaren inte är Microsoft?

Microsoft har stöd för Linux och teknik med öppen källkod i Azure. [Godkända Linux-distributioner](/azure/virtual-machines/linux/endorsed-distros) stöds i Azure och priset är integrerat i virtuella datorer. Eftersom Azure Linux-agenten redan är förinstallerad Azure Marketplace behandlas den som ett Microsoft-erbjudande. Eftersom Microsoft-erbjudanden godkänns som standard kan godkända Linux-distributioner inte hanteras i privata Azure Marketplace och godkänns som standard.

## <a name="contact-support"></a>Kontakta supporten

- Om Azure Marketplace support kan du besöka [Microsoft Q&A](/answers/products/).