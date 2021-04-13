---
title: Återställa administratörs behörighet för Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du kan hjälpa kunder att återställa en partners administratörs behörighet så att partnern kan hjälpa dig att hantera en kunds prenumeration på Azure CSP.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315855"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="0a34c-103">Återställa administratörs behörighet för en kunds Azure CSP-prenumeration</span><span class="sxs-lookup"><span data-stu-id="0a34c-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="0a34c-104">**Tillämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="0a34c-104">**Applicable roles**</span></span>

- <span data-ttu-id="0a34c-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="0a34c-105">Global admin</span></span>
- <span data-ttu-id="0a34c-106">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="0a34c-106">Admin agent</span></span>

<span data-ttu-id="0a34c-107">Som CSP-partner förväntar sig kunderna ofta att du ska hantera sin Azure-användning och deras system.</span><span class="sxs-lookup"><span data-stu-id="0a34c-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="0a34c-108">Om du gör det måste du ha administratörs behörighet.</span><span class="sxs-lookup"><span data-stu-id="0a34c-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="0a34c-109">Vissa behörigheter beviljas när din åter försäljares relation med kunden har upprättats.</span><span class="sxs-lookup"><span data-stu-id="0a34c-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="0a34c-110">Andra beviljas av kunden.</span><span class="sxs-lookup"><span data-stu-id="0a34c-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="0a34c-111">Administratörs behörighet för Azure i CSP</span><span class="sxs-lookup"><span data-stu-id="0a34c-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="0a34c-112">Det finns två nivåer av administratörs behörighet för Azure i CSP.</span><span class="sxs-lookup"><span data-stu-id="0a34c-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="0a34c-113">**Administratörs behörighet för klient organisation** (**delegerad administratörs behörighet**) – CSP-partner får de här privilegierna när du skapar en CSP-återförsäljares relation med kunder.</span><span class="sxs-lookup"><span data-stu-id="0a34c-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="0a34c-114">Delegerade administratörs privilegier ger CSP-partner åtkomst till sina kunders klienter, vilket gör att de kan utföra administrativa funktioner, till exempel lägga till/hantera användare, återställa lösen ord och hantera användar licenser.</span><span class="sxs-lookup"><span data-stu-id="0a34c-114">Delegated admin privileges gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="0a34c-115">**Administratörs behörighet på prenumerations nivå** – CSP-partners får de här behörigheterna när de skapar Azure CSP-prenumerationer för sina kunder.</span><span class="sxs-lookup"><span data-stu-id="0a34c-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="0a34c-116">Med dessa behörigheter får CSP-partner fullständig åtkomst till dessa prenumerationer, vilket gör att de kan etablera och hantera Azure-resurser.</span><span class="sxs-lookup"><span data-stu-id="0a34c-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="0a34c-117">Återställ administratörs behörighet för CSP-partner</span><span class="sxs-lookup"><span data-stu-id="0a34c-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="0a34c-118">Kunden kan återskapa CSP-rollens tilldelning så länge du anger objekt-ID: t för AdminAgents-gruppen till din kund.</span><span class="sxs-lookup"><span data-stu-id="0a34c-118">Your customer is able to re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="0a34c-119">Du måste arbeta med din kund för att återställa delegerade administratörs behörigheter.</span><span class="sxs-lookup"><span data-stu-id="0a34c-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="0a34c-120">Logga in på Partner Center-instrumentpanelen och välj **kunder** från menyn Partner Center.</span><span class="sxs-lookup"><span data-stu-id="0a34c-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="0a34c-121">Välj den kund som du arbetar med och **begär en åter försäljares relation.**</span><span class="sxs-lookup"><span data-stu-id="0a34c-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="0a34c-122">Detta genererar en länk till kunden som har administratörs behörighet för innehavare.</span><span class="sxs-lookup"><span data-stu-id="0a34c-122">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="0a34c-123">Kunden måste välja länken och godkänna åter försäljarens Relations förfrågan.</span><span class="sxs-lookup"><span data-stu-id="0a34c-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-postexempel för skapa åter försäljarens relation":::

4. <span data-ttu-id="0a34c-125">Du, partnern, måste ansluta till partner klienten för att hämta objekt-ID för AdminAgents-gruppen.</span><span class="sxs-lookup"><span data-stu-id="0a34c-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="0a34c-126">Din kund som har rollen **ägare eller administratör för användar åtkomst** och har behörighet att skapa roll tilldelning på prenumerations nivån gör följande:</span><span class="sxs-lookup"><span data-stu-id="0a34c-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="0a34c-127">Ansluter till den klient där CSP-prenumerationen finns.</span><span class="sxs-lookup"><span data-stu-id="0a34c-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="0a34c-128">Ansluter till prenumerationen (endast tillämpligt om användaren har roll tilldelnings behörigheter över flera prenumerationer i klienten).</span><span class="sxs-lookup"><span data-stu-id="0a34c-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="0a34c-129">PS C:\WINDOWS\system32> Set-AzContext-SubscriptionID prenumerations-ID för CSP ""</span><span class="sxs-lookup"><span data-stu-id="0a34c-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="0a34c-130">Skapar roll tilldelningen</span><span class="sxs-lookup"><span data-stu-id="0a34c-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="0a34c-131">Om du vill ge ägar rollen behörighet på resurs grupps nivå eller resurs nivå i stället för prenumerations omfånget kan följande kommandon fungera:</span><span class="sxs-lookup"><span data-stu-id="0a34c-131">If the desire is to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="0a34c-132">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="0a34c-132">Next steps</span></span>

- [<span data-ttu-id="0a34c-133">Hantera prenumerationer och resurser under Azure-planen</span><span class="sxs-lookup"><span data-stu-id="0a34c-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
