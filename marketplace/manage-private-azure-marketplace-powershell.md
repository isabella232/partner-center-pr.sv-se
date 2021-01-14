---
title: 'Snabb start: hantera en privat Azure Marketplace med PowerShell'
description: Den här snabb starten visar hur du hanterar erbjudanden på en privat Azure Marketplace med hjälp av Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d0021be17ab12b6e549b0e5263772a4a1e42f8a3
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182349"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="a9d70-103">Snabb start: hantera en privat Azure Marketplace med PowerShell</span><span class="sxs-lookup"><span data-stu-id="a9d70-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="a9d70-104">Den här artikeln beskriver hur du kan hantera erbjudanden i en privat Azure Marketplace med PowerShell-modulen [AZ. Marketplace](/powershell/module/az.marketplace) .</span><span class="sxs-lookup"><span data-stu-id="a9d70-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a9d70-105">Den privata Azure Marketplace är för närvarande en offentlig för hands version.</span><span class="sxs-lookup"><span data-stu-id="a9d70-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="a9d70-106">Förhandsversionen tillhandahålls utan serviceavtal.</span><span class="sxs-lookup"><span data-stu-id="a9d70-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="a9d70-107">Den rekommenderas inte för produktionsarbetsbelastningar.</span><span class="sxs-lookup"><span data-stu-id="a9d70-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="a9d70-108">Vissa funktioner kanske inte stöds eller kan ha begränsade funktioner.</span><span class="sxs-lookup"><span data-stu-id="a9d70-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="a9d70-109">Mer information finns i [Kompletterande villkor för användning av Microsoft Azure-förhandsversioner](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span><span class="sxs-lookup"><span data-stu-id="a9d70-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="a9d70-110">Krav</span><span class="sxs-lookup"><span data-stu-id="a9d70-110">Requirements</span></span>

* <span data-ttu-id="a9d70-111">Om du inte har en Azure-prenumeration kan du skapa ett [kostnadsfritt](https://azure.microsoft.com/free/) konto innan du börjar.</span><span class="sxs-lookup"><span data-stu-id="a9d70-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="a9d70-112">Om du väljer att använda Azure PowerShell lokalt:</span><span class="sxs-lookup"><span data-stu-id="a9d70-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="a9d70-113">[Installera AZ PowerShell-modulen](/powershell/azure/install-az-ps).</span><span class="sxs-lookup"><span data-stu-id="a9d70-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="a9d70-114">Anslut till ditt Azure-konto med hjälp av cmdleten [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) .</span><span class="sxs-lookup"><span data-stu-id="a9d70-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="a9d70-115">Om du väljer att använda Azure Cloud Shell:</span><span class="sxs-lookup"><span data-stu-id="a9d70-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="a9d70-116">Mer information finns i [Översikt över Azure Cloud Shell](/azure/cloud-shell/overview) .</span><span class="sxs-lookup"><span data-stu-id="a9d70-116">See [Overview of Azure Cloud Shell](/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="a9d70-117">Även om PowerShell-modulen **AZ. Marketplace** är i för hands version måste du installera den separat med hjälp av `Install-Module` cmdleten.</span><span class="sxs-lookup"><span data-stu-id="a9d70-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="a9d70-118">När modulen blir allmänt tillgänglig kommer den att ingå i framtida versioner av Az PowerShell-modulen och vara tillgänglig som standard i Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="a9d70-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="a9d70-119">Om du har flera Azure-prenumerationer väljer du lämplig prenumeration där resurserna ska faktureras.</span><span class="sxs-lookup"><span data-stu-id="a9d70-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="a9d70-120">Välj en speciell prenumeration med cmdleten [set-AzContext](/powershell/module/az.accounts/set-azcontext) .</span><span class="sxs-lookup"><span data-stu-id="a9d70-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="a9d70-121">Lista privata butiker</span><span class="sxs-lookup"><span data-stu-id="a9d70-121">List private stores</span></span>

<span data-ttu-id="a9d70-122">Om du vill hämta en lista över privata lager använder du cmdleten [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) .</span><span class="sxs-lookup"><span data-stu-id="a9d70-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="a9d70-123">I följande exempel visas privata butiker som har skapats under klient omfånget.</span><span class="sxs-lookup"><span data-stu-id="a9d70-123">The following example lists private stores that were created under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="a9d70-124">Lägg till ett erbjudande till en privat Marketplace</span><span class="sxs-lookup"><span data-stu-id="a9d70-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="a9d70-125">Om du vill lägga till ett erbjudande i ett privat lager använder du cmdleten [set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="a9d70-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="a9d70-126">I följande exempel läggs det angivna erbjudandet till i en privat Marketplace för en privat lagrings plats som skapas under klientens omfång.</span><span class="sxs-lookup"><span data-stu-id="a9d70-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a><span data-ttu-id="a9d70-127">Hämta erbjudanden för privata butiker</span><span class="sxs-lookup"><span data-stu-id="a9d70-127">Get private store offers</span></span>

<span data-ttu-id="a9d70-128">Om du vill hämta ett eller flera privata butiks erbjudanden använder du cmdleten [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="a9d70-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="a9d70-129">I följande exempel hämtas erbjudanden som är associerade med det angivna privata arkivet som lades till under klient omfånget.</span><span class="sxs-lookup"><span data-stu-id="a9d70-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a><span data-ttu-id="a9d70-130">Ta bort ett erbjudande</span><span class="sxs-lookup"><span data-stu-id="a9d70-130">Remove an offer</span></span>

<span data-ttu-id="a9d70-131">Om du vill ta bort ett erbjudande från ett privat lager använder du cmdleten [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="a9d70-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="a9d70-132">I följande exempel tas ett erbjudande bort från ett privat arkiv som har skapats i klient omfånget.</span><span class="sxs-lookup"><span data-stu-id="a9d70-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="a9d70-133">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="a9d70-133">Next steps</span></span>

<span data-ttu-id="a9d70-134">[Skapa och hantera privat Azure Marketplace](create-manage-private-azure-marketplace.md).</span><span class="sxs-lookup"><span data-stu-id="a9d70-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>