---
title: Storleksändring av virtuella Azure-datorer för maximal reservationsanvändning
description: Lär dig hur du ändrar storlek på en virtuell dator (VM) till dina kunders behov när du köper Microsoft Azure reservationer för dem.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 226ebd27b4ca4cdef56ce833a58a10bed89f8056
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534955"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Storleksändring av virtuell Microsoft Azure-dator för maximal reservationsanvändning

**Lämpliga roller**

- Administratörs agent
- Försäljnings agent

Den här artikeln förklarar hur du ändrar storlek på en virtuell dator (VM) till dina kunders behov när du köper Microsoft Azure reservationer för dem.
 
> [!NOTE]
> Den här artikeln gäller endast partner i Cloud Solution Provider (CSP)-programmet. Kunder som använder andra typer av prenumerationer (t. ex. betala per användning, enskilda, Microsoft-kundavtal eller Enterprise-avtal prenumerationer) bör i stället läsa [denna dokumentation om Azure-reservationer](/azure/cost-management-billing/reservations).

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Fastställa storleken på den virtuella datorn för en kunds Azure-reservation

När du köper Microsoft Azure reservationer för dina kunders räkning måste du välja en storlek för virtuella datorer (VM) för att uppfylla kundens data bearbetnings behov. Du kan hitta den här informationen på något av följande sätt:

- API för Azure-användning
- Azure Portal
- Azure PowerShell
- API för Azure Resource Manager (ARM)

Instruktioner för att använda var och en av dessa metoder finns nedan. När du har köpt en reservation tillämpas reservations rabatten automatiskt på virtuella datorer som matchar attributen och mängden av reservationen. Du behöver inte tilldela reservationen till en virtuell dator.

>[!NOTE]
>Reservations rabatter gäller inte för klassiska virtuella datorer eller reklam.

>[!IMPORTANT]
>För att korrekt identifiera typen och storleken på den virtuella datorn som ska köpas åt kunden, måste du använda en av de metoder som beskrivs nedan eftersom typen av VM-serien inte visas korrekt i filer för partner av Partner Center.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Hämta storleks information för virtuella datorer med Azures användnings-API

1. Använd värdet för attributet ServiceType från additionalInfo i API-svaret för att identifiera den VM-storlek som ska köpas.

2. Mer information finns i [Hämta en kunds användnings poster för Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) i [partner Center API](/partner-center/develop/).

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Hämta storleks information för virtuella datorer med hjälp av Microsoft Azure-portalen

1. Gå till sidan **kunder** i Partner Center.

2. Hitta kunden som vill köpa reservationer för virtuella Azure-datorer och välj sedan nedpilen för att expandera kundens information. Välj **Microsoft Azure-hanteringsportal** för att öppna kundens post i Azure Portal.

3. Välj **virtuella datorer** på Portal-menyn och välj sedan den virtuella dator som du vill köpa en reservation för.

4. På sidan information om den virtuella datorn hittar du storlek och regions information, enligt nedan, och använder den här informationen för att köpa reservationen i Partner Center.  

   :::image type="content" source="images/usage1.png" alt-text="Storlek och regions information på informations Sidan":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Hämta storleks information för virtuella datorer med Microsoft Azure PowerShell

Använd informationen i bilden nedan för att hämta platsen och storleken på den virtuella dator som du vill köpa en reservation för. 

:::image type="content" source="images/usage2.png" alt-text="VM-plats och storlek":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Hämta storleks information för virtuella datorer med hjälp av API: et för Azure Resource Manager (ARM)

1. Använd ARMClient eller ARM-API: erna för att anropa ARM-klienten för den virtuella dator som du vill köpa en reservation för.

2. /Subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-version = 2017-12-01

3. Anropet returnerar värdena för **vmSize** och **platsen**, enligt nedan.

    :::image type="content" source="images/usage3.png" alt-text="vmSize-värde":::
    :::image type="content" source="images/usage4.png" alt-text="plats värde":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Verifiera användningen av virtuella Azure-datorer och reservations rabatt

När du har köpt en Azure reserverad VM-instans för en kunds räkning, tillämpas rabatten för att betala för VM-utrymme i förväg automatiskt på de virtuella datorer som matchar attributen och antalet för kundens reservation.

Du kan kontrol lera kundens reservations användning och se vilka virtuella datorer som reservations rabatterna tillämpas på med hjälp av någon av följande metoder:

- Azure Portal
- API för Azure-användning

Instruktioner för att använda var och en av dessa metoder finns nedan.

>[!NOTE]
>Endast Azures användnings-API: et visar vilken virtuell dator som rabatten tillämpas på.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Verifiera kundens reservations användning i Microsoft Azure-portalen

1. Gå till sidan **kunder** i Partner Center.

2. Hitta kunden vars reservations rabatt och användning du vill verifiera och välj sedan nedpilen för att expandera kundens information. Välj **Microsoft Azure-hanteringsportal** för att öppna kundens post i Azure Portal.
3. Välj **reservationer** på Portal-menyn och välj sedan den reservation som du vill kontrol lera användningen för.
4. På sidan **Översikt** kontrollerar du diagrammets användnings diagram för reservationen, som visar hur mycket av reservationen som tillämpades på virtuella datorer.

    >[!NOTE]
    >Användnings data kan fördröjas med upp till 8 timmar.

    a. Om reservationens användning är 100% får kunden alla tänkbara besparingar som kan tillhandahållas av reservations köpet.
    b. Om reservationens användning är 0% används inte rabatten på någon virtuell dator.
    c. Om reservationens användning är mellan 1% och 99%, finns det några outnyttjade förmåner.

5. Undvik den här situationen genom att fastställa rätt storlek på den virtuella datorn som stöder kundens dator behov innan du gör köpet.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Verifiera kundens reservations användning med Azures API för användning

>[!NOTE]
>Endast Azures användnings-API: et visar vilken virtuell dator som rabatten tillämpas på.  

Du kan hämta reservations användnings data med Azure Usage API för att kontrol lera att kunden får reservations rabatten och se vilka virtuella datorer (virtuella datorer) som rabatten tillämpas på. Jämför exempel A till exempel B för att se hur du verifierar en kunds reservations användning.

:::image type="content" source="images/usage5.png" alt-text="Exempel på reservations användning":::

- ReservationId identifierar den Azure-reservation som användes för att tillämpa rabatten på den virtuella datorn.
- consumptionMeter är MeterId för den virtuella dator som har reservations rabatten som tillämpas.
- ReservationMeter visar $0-kostnaden sedan reservations Rabatten tillämpades.

Mer information finns i [Hämta en kunds användnings poster för Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) i [partner Center API](/partner-center/develop/).

>[!IMPORTANT]
>Program varu kostnader, till exempel Microsoft Windows Server, ingår för närvarande inte i priset för en VM-reservation och visas som separata rad objekt i order posten och på din faktura. Men om en kund har Azure Hybrid Use-förmånen kommer program kostnaden inte att tillämpas. Mer information finns i [Windows-programkostnader som inte ingår i reserverade instanser](/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="next-steps"></a>Nästa steg

|**För information om**   |**Läs detta**    |
|:-----------------------------|:-----------------|
|Översikt över Azure-reservationer i CSP  | [Sälj Microsoft Azure reserverade VM-instanser](azure-reservations.md)
|Köpa Azure-reservationer för dina kunder i Partner Center   | [Köp Azure-reservationer](azure-reservations-buying.md)
|Hantera Azure-reservationer i Partner Center | [Hantera Azure-reservationer i Partner Center](azure-reservations-manage.md)
|Köpa Azure-reservationer i Azure Portal | [Förskotts betalning för virtuella datorer med Azure Reserved VM instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) i Azure-hjälpen |
|Hantera Azure-reservationer i Azure Portal   | [Hantera reserverade VM-instanser](/azure/billing/billing-manage-reserved-vm-instance) i Azure-hjälpen  |
|Köpa Azure-reservationer med partner Center API | [Köp Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) i dokumentationen för partner Center-utvecklare   |
|Ge kunderna tillstånd att köpa sina egna Azure-reservationer från en prenumeration som du har köpt för dem. | [Ge kunderna tillstånd att köpa sina egna Azure-reservationer](give-customers-permission.md)   |