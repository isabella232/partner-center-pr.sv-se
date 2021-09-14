---
title: 'Snabbstart: Hantera en privat Azure Marketplace powershell'
description: Den här snabbstarten visar hur du hanterar erbjudanden i en privat Azure Marketplace med Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.service: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d7bd790eab2618822dbc5099ad1ad107794c82d2
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246666"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a>Snabbstart: Hantera en privat Azure Marketplace powershell

Den här artikeln beskriver hur du kan hantera erbjudanden i en privat Azure Marketplace med hjälp av [Az.Marketplace](/powershell/module/az.marketplace) PowerShell-modulen.

> [!IMPORTANT]
> Privata Azure Marketplace är för närvarande i offentlig förhandsversion. Förhandsversionen tillhandahålls utan serviceavtal. Den rekommenderas inte för produktionsarbetsbelastningar. Vissa funktioner kanske inte stöds eller har begränsade funktioner. Mer information finns i [Kompletterande villkor för användning av Microsoft Azure-förhandsversioner](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).

## <a name="requirements"></a>Krav

* Om du inte har en Azure-prenumeration kan du skapa ett [kostnadsfritt](https://azure.microsoft.com/free/) konto innan du börjar.

* Om du väljer att använda Azure PowerShell lokalt:
  * [Installera Az PowerShell-modulen](/powershell/azure/install-az-ps).
  * Anslut till ditt Azure-konto [med cmdleten Anslut-AzAccount.](/powershell/module/az.accounts/connect-azaccount)
* Om du väljer att använda Azure Cloud Shell:
  * Se [Översikt över Azure Cloud Shell](/azure/cloud-shell/overview) för mer information.

  > [!IMPORTANT]
  > När **Az.Marketplace** PowerShell-modulen är i förhandsversion måste du installera den separat med hjälp av `Install-Module` cmdleten . När modulen blir allmänt tillgänglig kommer den att ingå i framtida versioner av Az PowerShell-modulen och vara tillgänglig som standard i Azure Cloud Shell.

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* Om du har flera Azure-prenumerationer väljer du lämplig prenumeration där resurserna ska debiteras. Välj en specifik prenumeration med hjälp [av cmdleten Set-AzContext.](/powershell/module/az.accounts/set-azcontext)

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a>Lista privata butiker

Om du vill hämta en lista över privata butiker använder du cmdleten [Get-AzMarketplacePrivateStore.](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) I följande exempel visas privata butiker som har skapats under klientorganisationsomfånget.

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

## <a name="add-an-offer-to-a-private-marketplace"></a>Lägga till ett erbjudande på en privat marknadsplats

Om du vill lägga till ett erbjudande i en privat butik använder du cmdleten [Set-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) I följande exempel läggs det angivna erbjudandet till på en privat marknadsplats för en privat butik som skapas under klientorganisationsomfånget.

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

## <a name="get-private-store-offers"></a>Skaffa privata butikserbjudanden

Om du vill hämta ett eller flera privata butikserbjudanden använder du cmdleten [Get-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) I följande exempel hämtar erbjudanden som är associerade med det angivna privata arkivet som har lagts till under klientorganisationsomfånget.

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

## <a name="remove-an-offer"></a>Ta bort ett erbjudande

Om du vill ta bort ett erbjudande från en privat butik använder du cmdleten [Remove-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) I följande exempel tas ett erbjudande bort från ett privat arkiv som har skapats i klientorganisationsomfånget.

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a>Nästa steg

[Skapa och hantera privata Azure Marketplace](create-manage-private-azure-marketplace.md).