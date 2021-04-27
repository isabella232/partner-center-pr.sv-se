---
title: Återställa administratörsbehörighet för Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du hjälper kunder att återställa en partners administratörsbehörighet så att partnern kan hjälpa till att hantera en kunds Azure CSP prenumerationer.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018195"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="6dcec-103">Återställa administratörsbehörigheter för en kunds Azure CSP prenumerationer</span><span class="sxs-lookup"><span data-stu-id="6dcec-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="6dcec-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="6dcec-104">**Appropriate roles**</span></span>

- <span data-ttu-id="6dcec-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="6dcec-105">Global admin</span></span>
- <span data-ttu-id="6dcec-106">Administratörsagent</span><span class="sxs-lookup"><span data-stu-id="6dcec-106">Admin agent</span></span>

<span data-ttu-id="6dcec-107">Som CSP-partner förväntar sig kunderna ofta att du hanterar deras Azure-användning och deras system åt dem.</span><span class="sxs-lookup"><span data-stu-id="6dcec-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="6dcec-108">Om du gör det måste du ha administratörsbehörighet.</span><span class="sxs-lookup"><span data-stu-id="6dcec-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="6dcec-109">Vissa behörigheter beviljas när din återförsäljarrelation med kunden upprättas.</span><span class="sxs-lookup"><span data-stu-id="6dcec-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="6dcec-110">Andra beviljas till dig av din kund.</span><span class="sxs-lookup"><span data-stu-id="6dcec-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="6dcec-111">Administratörsbehörighet för Azure i CSP</span><span class="sxs-lookup"><span data-stu-id="6dcec-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="6dcec-112">Det finns två nivåer av administratörsbehörighet för Azure i CSP.</span><span class="sxs-lookup"><span data-stu-id="6dcec-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="6dcec-113">**Administratörsbehörigheter på klientorganisationsnivå** **(delegerade administratörsbehörigheter)**– CSP-partner får dessa privilegier när de upprättar en CSP-återförsäljarrelation med kunder.</span><span class="sxs-lookup"><span data-stu-id="6dcec-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="6dcec-114">Delegerade administratörsbehörigheter ger CSP-partner åtkomst till sina kunders klienter, vilket gör att de kan utföra administrativa funktioner som att lägga till/hantera användare, återställa lösenord och hantera användarlicenser.</span><span class="sxs-lookup"><span data-stu-id="6dcec-114">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="6dcec-115">**Administratörsbehörighet på prenumerationsnivå** – CSP-partner får dessa behörigheter när de skapar Azure CSP prenumerationer för sina kunder.</span><span class="sxs-lookup"><span data-stu-id="6dcec-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="6dcec-116">Med dessa behörigheter får CSP-partner fullständig åtkomst till dessa prenumerationer, vilket gör att de kan etablera och hantera Azure-resurser.</span><span class="sxs-lookup"><span data-stu-id="6dcec-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="6dcec-117">Återställa CSP-partners administratörsbehörigheter</span><span class="sxs-lookup"><span data-stu-id="6dcec-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="6dcec-118">Kunden kan skapa CSP-rolltilldelningen på nytt så länge du anger objekt-ID:t för gruppen AdminAgents till kunden.</span><span class="sxs-lookup"><span data-stu-id="6dcec-118">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="6dcec-119">Om du vill återfå delegerade administratörsbehörigheter måste du arbeta med kunden.</span><span class="sxs-lookup"><span data-stu-id="6dcec-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="6dcec-120">Logga in på instrumentpanelen i Partnercenter och välj Kunder i **Partnercenter-menyn.**</span><span class="sxs-lookup"><span data-stu-id="6dcec-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="6dcec-121">Välj den kund som du arbetar med och **begär en återförsäljarrelation.**</span><span class="sxs-lookup"><span data-stu-id="6dcec-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="6dcec-122">Den här åtgärden genererar en länk till kunden som har administratörsrättigheter för klientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="6dcec-122">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="6dcec-123">Kunden måste välja länken och godkänna begäran om återförsäljarrelation.</span><span class="sxs-lookup"><span data-stu-id="6dcec-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-postexempel för att skapa återförsäljarrelation":::

4. <span data-ttu-id="6dcec-125">Du, partnern, måste ansluta till partnerklientorganisationen för att hämta objekt-ID för gruppen AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="6dcec-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="6dcec-126">Kunden som har rollen ägare eller administratör **för användaråtkomst** och har behörighet att skapa rolltilldelningar på prenumerationsnivå gör följande:</span><span class="sxs-lookup"><span data-stu-id="6dcec-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="6dcec-127">Ansluter till den klientorganisation där CSP-prenumerationen finns.</span><span class="sxs-lookup"><span data-stu-id="6dcec-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="6dcec-128">Ansluter till prenumerationen (gäller endast om användaren har rolltilldelningsbehörigheter över flera prenumerationer i klientorganisationen).</span><span class="sxs-lookup"><span data-stu-id="6dcec-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="6dcec-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"'</span><span class="sxs-lookup"><span data-stu-id="6dcec-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="6dcec-130">Skapar rolltilldelningen</span><span class="sxs-lookup"><span data-stu-id="6dcec-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="6dcec-131">Om du vill ge ägarrollen behörighet på resursgruppsnivå eller resursnivå i stället för prenumerationsomfånget kan följande kommandon fungera:</span><span class="sxs-lookup"><span data-stu-id="6dcec-131">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="6dcec-132">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="6dcec-132">Next steps</span></span>

- [<span data-ttu-id="6dcec-133">Hantera prenumerationer och resurser under Azure-planen</span><span class="sxs-lookup"><span data-stu-id="6dcec-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
