---
title: Storleksändring av virtuella Azure-datorer för maximal reservationsanvändning
description: Lär dig att ändra storlek på en virtuell dator (VM) till dina kunders databehandlingsbehov när du köper Microsoft Azure reservationer åt dem.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: dc9b9100e01191c24c03c76e9a9ff5a6ffe335d1
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246325"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Storleksändring av virtuell Microsoft Azure-dator för maximal reservationsanvändning

**Lämpliga roller:** Administratörsagent | Försäljningsagent

I den här artikeln förklaras hur du kan ändra storlek på en virtuell dator (VM) till dina kunders databehandlingsbehov när du köper Microsoft Azure reservationer åt dem.
 
> [!NOTE]
> Den här artikeln gäller endast för partner i Molnlösningsleverantör-programmet (CSP). Kunder som använder andra typer av prenumerationer (till exempel betala enligt användning, enskilda prenumerationer, Microsoft-kundavtal eller företagsavtal-prenumerationer) bör i stället läsa dokumentationen om [Azure-reservationer.](/azure/cost-management-billing/reservations)

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Fastställa VM-storleken för en kunds Azure-reservation

När du Microsoft Azure reservationer åt dina kunder måste du välja en virtuell dator (VM) som uppfyller kundens databehandlingsbehov. Du hittar den här informationen med någon av följande metoder:

- API för Azure-användning
- Azure Portal
- Azure PowerShell
- ARM-API:et (Azure Resource Manager)

Anvisningar för hur du använder var och en av dessa metoder finns nedan. När du har köpt en reservation tillämpas reservationsrabatten automatiskt på virtuella datorer som matchar reservationens attribut och kvantitet. Du behöver inte tilldela reservationen till en virtuell dator.

>[!NOTE]
>Reservationsrabatter gäller inte för klassiska eller kampanj-VM:ar.

>[!IMPORTANT]
>För att korrekt identifiera typen och storleken på den virtuella dator som du ska köpa för din kunds räkning måste du använda någon av metoderna som beskrivs nedan eftersom VM-serietypen inte visas korrekt i Partner Center-avstämningsfiler.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Hämta storleksinformation för virtuella datorer med hjälp av API:et för Azure-användning

1. Använd värdet för ServiceType-attributet från additionalInfo i API-svaret för att identifiera vm-storleken som ska köpas.

2. Mer information finns i [Hämta en kunds användningsposter för Azure i](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) Partner Center [API.](/partner-center/develop/)

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Hämta storleksinformation för virtuella datorer med hjälp Microsoft Azure portalen

1. I Partnercenter går du till sidan **Kunder.**

2. Hitta den kund som vill köpa reservationer för virtuella Azure-datorer och välj sedan nedåtpilen för att expandera kundens information. Välj **Microsoft Azure Hanteringsportal** för att öppna kundens post i Azure Portal.

3. Välj **Virtuella datorer** på portalmenyn och välj sedan den virtuella dator som du vill köpa en reservation för.

4. På den virtuella datorns informationssida hittar du storleks- och regionsinformationen, som visas nedan, och använder den här informationen för att köpa reservationen i Partnercenter.  

   :::image type="content" source="images/usage1.png" alt-text="Information om storlek och region på detaljsidan.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Hämta storleksinformation för virtuella datorer med Microsoft Azure PowerShell

Använd informationen i bilden nedan för att hämta platsen och storleken på den virtuella dator som du vill köpa en reservation för. 

:::image type="content" source="images/usage2.png" alt-text="Plats och storlek för virtuell dator.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Hämta storleksinformation för virtuella datorer med hjälp Azure Resource Manager (ARM) API

1. Med ARMClient eller ARM-API:erna anropar du ARM-klienten för den virtuella dator som du vill köpa en reservation för.

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. Anropet returnerar värdena **för vmSize** **och location**, som du ser nedan.

    :::image type="content" source="images/usage3.png" alt-text="vmSize-värde.":::
    :::image type="content" source="images/usage4.png" alt-text="platsvärde.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Kontrollera användningen av virtuella Azure-datorer och reservationsrabatten

När du har köpt en azure-reserverad VM-instans åt en kund tillämpas rabatten för att betala för VM-utrymme i förväg automatiskt på de virtuella datorer som matchar attributen och kvantiteten för kundens reservation.

Du kan kontrollera kundens reservationsanvändning och se vilka virtuella datorer reservationsrabatterna tillämpas på med någon av följande metoder:

- Azure Portal
- API för Azure-användning

Anvisningar för hur du använder var och en av dessa metoder finns nedan.

>[!NOTE]
>Endast API:et för Azure-användning visar vilken virtuell dator rabatten tillämpas på.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Verifiera kundens reservationsanvändning i Microsoft Azure portalen

1. I Partnercenter går du till sidan **Kunder.**

2. Hitta den kund vars reservationsrabatt och användning du vill verifiera och välj sedan nedåtpilen för att expandera kundens information. Välj **Microsoft Azure Hanteringsportal** för att öppna kundens post i Azure Portal.
3. Välj **Reservationer** på portalmenyn och välj sedan den reservation som du vill kontrollera användningen för.
4. På sidan **Översikt** kontrollerar du reservationens användningsdiagram, som visar hur mycket av reservationen som tillämpades på virtuella datorer.

    >[!NOTE]
    >Användningsdata kan fördröjas med upp till 8 timmar.

    a. Om reservationens utnyttjande är 100 % får kunden alla möjliga besparingar som reservationsköpet kan ge.
    b. Om reservationens användning är 0 % tillämpas rabatten inte på någon virtuell dator.
    c. Om reservationens användning är mellan 1 % och 99 % finns det oanvända fördelar.

5. Undvik den här situationen genom att fastställa rätt storlek på den virtuella datorn för att stödja kundens behov av databehandling innan köpet.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Verifiera kundens reservationsanvändning med API:et för Azure-användning

>[!NOTE]
>Endast API:et för Azure-användning visar vilken virtuell dator rabatten tillämpas på.  

Du kan hämta användningsdata för reservationer med API:et för Azure-användning för att kontrollera att kunden får reservationsrabatten och för att se vilka virtuella datorer som rabatten tillämpas på. Jämför exempel A med exempel B för att se hur du verifierar en kunds reservationsanvändning.

:::image type="content" source="images/usage5.png" alt-text="Exempel på reservationsanvändning.":::

- reservationId identifierar den Azure-reservation som användes för att tillämpa rabatten på den virtuella datorn.
- consumptionMeter är MeterId för den virtuella dator där reservationsrabatten tillämpas.
- ReservationMeter visar en kostnad på 0 USD sedan reservationsrabatten tillämpades.

Mer information finns i [Hämta en kunds användningsposter för Azure i](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) Partner Center [API.](/partner-center/develop/)

>[!IMPORTANT]
>Programvarukostnader, till exempel Microsoft Windows Server, ingår för närvarande inte i priset för en VM-reservation och visas som separata radobjekt i orderposten och på fakturan. Men om en kund har Azure Hybrid Use Benefit tillämpas inte programvarukostnaderna. Mer information finns i [Windows programvarukostnader som inte ingår i reserverade instanser.](/azure/billing/billing-reserved-instance-windows-software-costs)  

## <a name="next-steps"></a>Nästa steg

|**För information om**   |**Läs detta**    |
|:-----------------------------|:-----------------|
|Översikt över Azure-reservationer i CSP  | [Sälja Microsoft Azure reserverade VM-instanser](azure-reservations.md)
|Köpa Azure-reservationer för dina kunder i Partnercenter   | [Köpa Azure-reservationer](azure-reservations-buying.md)
|Hantera Azure-reservationer i Partnercenter | [Hantera Azure-reservationer i Partnercenter](azure-reservations-manage.md)
|Köpa Azure-reservationer i Azure Portal | [Förskottsbetala för virtuella datorer Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) i Azure-hjälpen |
|Hantera Azure-reservationer i Azure Portal   | [Hantera reserverade VM-instanser](/azure/billing/billing-manage-reserved-vm-instance) i Azure-hjälpen  |
|Köpa Azure-reservationer med partnercenter-API:et | [Köp Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) i utvecklardokumentationen för Partnercenter   |
|Ge kunderna tillstånd att köpa sina egna Azure-reservationer från en prenumeration som du har köpt åt dem. | [Ge kunderna behörighet att köpa sina egna Azure-reservationer](give-customers-permission.md)   |