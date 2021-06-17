---
title: Återställa administratörsbehörigheter för Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du hjälper kunder att återställa en partners administratörsbehörighet så att partnern kan hantera en kunds Azure CSP prenumerationer.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 81df7578f7f15def64a3c20b15f95f3b89a28d1c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277784"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="205e9-103">Återställa administratörsbehörigheter för en kunds Azure CSP prenumerationer</span><span class="sxs-lookup"><span data-stu-id="205e9-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="205e9-104">**Lämpliga roller:** Globala | Administratörsagent</span><span class="sxs-lookup"><span data-stu-id="205e9-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="205e9-105">Som CSP-partner förväntar sig kunderna ofta att du hanterar deras Azure-användning och deras system åt dem.</span><span class="sxs-lookup"><span data-stu-id="205e9-105">As a CSP partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="205e9-106">Du måste ha administratörsbehörighet för att göra det.</span><span class="sxs-lookup"><span data-stu-id="205e9-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="205e9-107">Vissa behörigheter beviljas när din återförsäljarrelation med kunden upprättas.</span><span class="sxs-lookup"><span data-stu-id="205e9-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="205e9-108">Andra beviljas till dig av din kund.</span><span class="sxs-lookup"><span data-stu-id="205e9-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="205e9-109">Administratörsbehörighet för Azure i CSP</span><span class="sxs-lookup"><span data-stu-id="205e9-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="205e9-110">Det finns två nivåer av administratörsbehörighet för Azure i CSP.</span><span class="sxs-lookup"><span data-stu-id="205e9-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="205e9-111">**Administratörsbehörighet på klientorganisationsnivå (delegerade administratörsbehörigheter):** CSP-partner får dessa behörigheter när de upprättar en CSP-återförsäljarrelation med kunder.</span><span class="sxs-lookup"><span data-stu-id="205e9-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="205e9-112">Delegerade administratörsbehörigheter ger CSP-partner åtkomst till sina kunders klienter.</span><span class="sxs-lookup"><span data-stu-id="205e9-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="205e9-113">Den här åtkomsten gör att de kan använda administrativa funktioner som att lägga till/hantera användare, återställa lösenord och hantera användarlicenser.</span><span class="sxs-lookup"><span data-stu-id="205e9-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="205e9-114">**Administratörsbehörighet på prenumerationsnivå:** CSP-partner får dessa behörigheter när de skapar Azure CSP prenumerationer för sina kunder.</span><span class="sxs-lookup"><span data-stu-id="205e9-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="205e9-115">Dessa behörigheter ger CSP-partner fullständig åtkomst till dessa prenumerationer, vilket gör att de kan etablera och hantera Azure-resurser.</span><span class="sxs-lookup"><span data-stu-id="205e9-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="205e9-116">Återställa CSP:ens administratörsbehörighet</span><span class="sxs-lookup"><span data-stu-id="205e9-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="205e9-117">Kunden kan skapa CSP-rolltilldelningen på nytt om du anger `object ID` för gruppen AdminAgents till kunden.</span><span class="sxs-lookup"><span data-stu-id="205e9-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="205e9-118">För att återfå delegerade administratörsbehörigheter måste du arbeta med kunden genom följande steg.</span><span class="sxs-lookup"><span data-stu-id="205e9-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="205e9-119">Logga in på instrumentpanelen i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="205e9-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="205e9-120">På menyn i Partnercenter väljer du **Kunder.**</span><span class="sxs-lookup"><span data-stu-id="205e9-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="205e9-121">Välj den kund som du arbetar med och **begär en återförsäljarrelation**.</span><span class="sxs-lookup"><span data-stu-id="205e9-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="205e9-122">Den här åtgärden genererar en länk till kunden som har administratörsrättigheter för klientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="205e9-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="205e9-123">Kunden måste välja länken och godkänna begäran om återförsäljarrelation.</span><span class="sxs-lookup"><span data-stu-id="205e9-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-postexempel för att skapa återförsäljarrelation.":::

5. <span data-ttu-id="205e9-125">Du, partnern, måste ansluta till partnerklientorganisationen för att hämta objekt-ID för gruppen AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="205e9-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="205e9-126">Kunden måste sedan göra följande med antingen PowerShell eller Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="205e9-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="205e9-127">Kunden måste ha:</span><span class="sxs-lookup"><span data-stu-id="205e9-127">Your customer must have:</span></span>

- <span data-ttu-id="205e9-128">Rollen som ägare **eller** administratör **för användaråtkomst**</span><span class="sxs-lookup"><span data-stu-id="205e9-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="205e9-129">Behörigheter för att skapa rolltilldelningar på prenumerationsnivå</span><span class="sxs-lookup"><span data-stu-id="205e9-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="205e9-130">a.</span><span class="sxs-lookup"><span data-stu-id="205e9-130">a.</span></span> <span data-ttu-id="205e9-131">Endast för PowerShell måste kunden uppdatera `Az.Resources` modulen.</span><span class="sxs-lookup"><span data-stu-id="205e9-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="205e9-132">b.</span><span class="sxs-lookup"><span data-stu-id="205e9-132">b.</span></span> <span data-ttu-id="205e9-133">Kunden ansluter till den klientorganisation där CSP-prenumerationen finns.</span><span class="sxs-lookup"><span data-stu-id="205e9-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="205e9-134">c.</span><span class="sxs-lookup"><span data-stu-id="205e9-134">c.</span></span> <span data-ttu-id="205e9-135">Kunden ansluter till prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="205e9-135">The customer connects to the subscription.</span></span> <span data-ttu-id="205e9-136">Detta gäller *endast* om användaren har rolltilldelningsbehörigheter över flera prenumerationer i klientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="205e9-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="205e9-137">d.</span><span class="sxs-lookup"><span data-stu-id="205e9-137">d.</span></span> <span data-ttu-id="205e9-138">Kunden skapar sedan rolltilldelningen.</span><span class="sxs-lookup"><span data-stu-id="205e9-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="205e9-139">I stället för att bevilja ägarbehörighet för prenumerationsomfånget kan du bevilja på resursgrupps- eller resursnivå.</span><span class="sxs-lookup"><span data-stu-id="205e9-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="205e9-140">På resursgruppsnivå</span><span class="sxs-lookup"><span data-stu-id="205e9-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="205e9-141">På resursnivå</span><span class="sxs-lookup"><span data-stu-id="205e9-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="205e9-142">Om ovanstående steg inte fungerar eller om du får felmeddelanden när du försöker dem kan du prova följande "catch-all"-procedur för att återställa administratörsrättigheter för din kund.</span><span class="sxs-lookup"><span data-stu-id="205e9-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="205e9-143">Felsökning</span><span class="sxs-lookup"><span data-stu-id="205e9-143">Troubleshooting</span></span>

<span data-ttu-id="205e9-144">Om kunden inte kan slutföra steg 6 ovan kan kunden prova följande kommando:</span><span class="sxs-lookup"><span data-stu-id="205e9-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="205e9-145">Ange den resulterande `newRoleAssignment.log` filen till Microsoft för ytterligare analys.</span><span class="sxs-lookup"><span data-stu-id="205e9-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="205e9-146">Om "catch-all"-proceduren misslyckas under `Import-Module` kan du prova följande steg:</span><span class="sxs-lookup"><span data-stu-id="205e9-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="205e9-147">Om importen misslyckas eftersom modulen används startar du om PowerShell-sessionen genom att stänga och öppna alla fönster igen.</span><span class="sxs-lookup"><span data-stu-id="205e9-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="205e9-148">Kontrollera versionen av `Az.Resources` med `Get-Module Az.Resources -ListAvailable` .</span><span class="sxs-lookup"><span data-stu-id="205e9-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="205e9-149">Om version 4.1.1 inte finns i den tillgängliga listan måste du använda `Update-Module Az.Resources -Force` .</span><span class="sxs-lookup"><span data-stu-id="205e9-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="205e9-150">Om felet visar att `Az.Accounts` måste vara en specifik version uppdaterar du även den modulen och ersätter `Az.Resources` med `Az.Accounts` .</span><span class="sxs-lookup"><span data-stu-id="205e9-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="205e9-151">Du måste sedan starta om PowerShell-sessionen.</span><span class="sxs-lookup"><span data-stu-id="205e9-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="205e9-152">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="205e9-152">Next steps</span></span>

- [<span data-ttu-id="205e9-153">Hantera prenumerationer och resurser under Azure-planen</span><span class="sxs-lookup"><span data-stu-id="205e9-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
