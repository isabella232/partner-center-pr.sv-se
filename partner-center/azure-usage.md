---
title: Storleksändring av virtuella Azure-datorer för maximal reservationsanvändning
description: Lär dig att ändra storlek på en virtuell dator (VM) efter dina kunders databehandlingsbehov när du köper Microsoft Azure reservationer åt dem.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 650618de7460f4667c60ac58cbe6716530db7f16
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510201"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="32d3f-103">Storleksändring av virtuell Microsoft Azure-dator för maximal reservationsanvändning</span><span class="sxs-lookup"><span data-stu-id="32d3f-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="32d3f-104">**Lämpliga roller:** Administratörsagent | Försäljningsagent</span><span class="sxs-lookup"><span data-stu-id="32d3f-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="32d3f-105">I den här artikeln förklaras hur du kan ändra storlek på en virtuell dator (VM) till dina kunders databehandlingsbehov när du köper Microsoft Azure reservationer åt dem.</span><span class="sxs-lookup"><span data-stu-id="32d3f-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="32d3f-106">Den här artikeln gäller endast för partner i Molnlösningsleverantör-programmet (CSP).</span><span class="sxs-lookup"><span data-stu-id="32d3f-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="32d3f-107">Kunder som använder andra typer av prenumerationer (till exempel betala enligt användning, enskilda prenumerationer, Microsoft-kundavtal- eller företagsavtal-prenumerationer) bör i stället läsa dokumentationen om [Azure-reservationer.](/azure/cost-management-billing/reservations)</span><span class="sxs-lookup"><span data-stu-id="32d3f-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="32d3f-108">Fastställa VM-storleken för en kunds Azure-reservation</span><span class="sxs-lookup"><span data-stu-id="32d3f-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="32d3f-109">När du Microsoft Azure en reservation åt dina kunder måste du välja en virtuell dator (VM) som uppfyller kundens databehandlingsbehov.</span><span class="sxs-lookup"><span data-stu-id="32d3f-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="32d3f-110">Du hittar den här informationen på något av följande sätt:</span><span class="sxs-lookup"><span data-stu-id="32d3f-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="32d3f-111">API för Azure-användning</span><span class="sxs-lookup"><span data-stu-id="32d3f-111">Azure utilization API</span></span>
- <span data-ttu-id="32d3f-112">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="32d3f-112">The Azure portal</span></span>
- <span data-ttu-id="32d3f-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="32d3f-113">Azure PowerShell</span></span>
- <span data-ttu-id="32d3f-114">ARM-API:et (Azure Resource Manager)</span><span class="sxs-lookup"><span data-stu-id="32d3f-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="32d3f-115">Anvisningar för hur du använder var och en av dessa metoder finns nedan.</span><span class="sxs-lookup"><span data-stu-id="32d3f-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="32d3f-116">När du har köpt en reservation tillämpas reservationsrabatten automatiskt på virtuella datorer som matchar reservationens attribut och kvantitet.</span><span class="sxs-lookup"><span data-stu-id="32d3f-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="32d3f-117">Du behöver inte tilldela reservationen till en virtuell dator.</span><span class="sxs-lookup"><span data-stu-id="32d3f-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="32d3f-118">Reservationsrabatter gäller inte för klassiska eller kampanj-VM:ar.</span><span class="sxs-lookup"><span data-stu-id="32d3f-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="32d3f-119">För att korrekt identifiera typen och storleken på den virtuella dator som du ska köpa för din kunds räkning måste du använda någon av metoderna som beskrivs nedan eftersom VM-serietypen inte visas korrekt i Avstämningsfiler för Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="32d3f-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="32d3f-120">Hämta storleksinformation för virtuella datorer med hjälp av API:et för Azure-användning</span><span class="sxs-lookup"><span data-stu-id="32d3f-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="32d3f-121">Använd värdet för ServiceType-attributet från additionalInfo i API-svaret för att identifiera vm-storleken som ska köpas.</span><span class="sxs-lookup"><span data-stu-id="32d3f-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="32d3f-122">Mer information finns i [Hämta en kunds användningsposter för Azure i](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) Partner Center [API.](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="32d3f-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="32d3f-123">Hämta storleksinformation för virtuella datorer med hjälp Microsoft Azure portalen</span><span class="sxs-lookup"><span data-stu-id="32d3f-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="32d3f-124">I Partnercenter går du till sidan **Kunder.**</span><span class="sxs-lookup"><span data-stu-id="32d3f-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="32d3f-125">Hitta den kund som vill köpa reservationer för virtuella Azure-datorer och välj sedan nedåtpilen för att expandera kundens information.</span><span class="sxs-lookup"><span data-stu-id="32d3f-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="32d3f-126">Välj **Microsoft Azure Hanteringsportal** för att öppna kundens post i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="32d3f-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="32d3f-127">Välj **Virtuella datorer** på portalmenyn och välj sedan den virtuella dator som du vill köpa en reservation för.</span><span class="sxs-lookup"><span data-stu-id="32d3f-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="32d3f-128">På den virtuella datorns informationssida hittar du storleks- och regionsinformationen, som visas nedan, och använder den här informationen för att köpa reservationen i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="32d3f-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Information om storlek och region på detaljsidan.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="32d3f-130">Hämta storleksinformation för virtuella datorer med Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="32d3f-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="32d3f-131">Använd informationen i bilden nedan för att hämta platsen och storleken på den virtuella dator som du vill köpa en reservation för.</span><span class="sxs-lookup"><span data-stu-id="32d3f-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Vm-plats och storlek.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="32d3f-133">Hämta storleksinformation för virtuella datorer med hjälp av AZURE RESOURCE MANAGER-API:et (ARM)</span><span class="sxs-lookup"><span data-stu-id="32d3f-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="32d3f-134">Med ARMClient eller ARM-API:erna anropar du ARM-klienten för den virtuella dator som du vill köpa en reservation för.</span><span class="sxs-lookup"><span data-stu-id="32d3f-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. <span data-ttu-id="32d3f-135">Anropet returnerar värdena **för vmSize** **och location**, som du ser nedan.</span><span class="sxs-lookup"><span data-stu-id="32d3f-135">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize-värde.":::
    :::image type="content" source="images/usage4.png" alt-text="platsvärde.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="32d3f-138">Kontrollera användningen av virtuella Azure-datorer och reservationsrabatten</span><span class="sxs-lookup"><span data-stu-id="32d3f-138">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="32d3f-139">När du har köpt en azure-reserverad VM-instans åt en kund tillämpas rabatten för att betala för VM-utrymme i förväg automatiskt på de virtuella datorer som matchar attributen och kvantiteten för kundens reservation.</span><span class="sxs-lookup"><span data-stu-id="32d3f-139">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="32d3f-140">Du kan kontrollera kundens reservationsanvändning och se vilka virtuella datorer reservationsrabatterna tillämpas på med någon av följande metoder:</span><span class="sxs-lookup"><span data-stu-id="32d3f-140">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="32d3f-141">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="32d3f-141">The Azure portal</span></span>
- <span data-ttu-id="32d3f-142">API för Azure-användning</span><span class="sxs-lookup"><span data-stu-id="32d3f-142">Azure utilization API</span></span>

<span data-ttu-id="32d3f-143">Anvisningar för hur du använder var och en av dessa metoder finns nedan.</span><span class="sxs-lookup"><span data-stu-id="32d3f-143">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="32d3f-144">Endast API:et för Azure-användning visar vilken virtuell dator rabatten tillämpas på.</span><span class="sxs-lookup"><span data-stu-id="32d3f-144">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="32d3f-145">Kontrollera kundens reservationsanvändning i Microsoft Azure portalen</span><span class="sxs-lookup"><span data-stu-id="32d3f-145">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="32d3f-146">I Partnercenter går du till sidan **Kunder.**</span><span class="sxs-lookup"><span data-stu-id="32d3f-146">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="32d3f-147">Hitta den kund vars reservationsrabatt och användning du vill verifiera och välj sedan nedåtpilen för att expandera kundens information.</span><span class="sxs-lookup"><span data-stu-id="32d3f-147">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="32d3f-148">Välj **Microsoft Azure Hanteringsportal** för att öppna kundens post i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="32d3f-148">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="32d3f-149">Välj **Reservationer** på portalmenyn och välj sedan den reservation som du vill kontrollera användningen för.</span><span class="sxs-lookup"><span data-stu-id="32d3f-149">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="32d3f-150">På sidan **Översikt** kontrollerar du reservationens användningsdiagram, som visar hur mycket av reservationen som tillämpades på virtuella datorer.</span><span class="sxs-lookup"><span data-stu-id="32d3f-150">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="32d3f-151">Användningsdata kan fördröjas med upp till 8 timmar.</span><span class="sxs-lookup"><span data-stu-id="32d3f-151">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="32d3f-152">a.</span><span class="sxs-lookup"><span data-stu-id="32d3f-152">a.</span></span> <span data-ttu-id="32d3f-153">Om reservationens användning är 100 % får kunden alla möjliga besparingar som reservationsköpet kan ge.</span><span class="sxs-lookup"><span data-stu-id="32d3f-153">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="32d3f-154">b.</span><span class="sxs-lookup"><span data-stu-id="32d3f-154">b.</span></span> <span data-ttu-id="32d3f-155">Om reservationens användning är 0 % tillämpas rabatten inte på någon virtuell dator.</span><span class="sxs-lookup"><span data-stu-id="32d3f-155">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="32d3f-156">c.</span><span class="sxs-lookup"><span data-stu-id="32d3f-156">c.</span></span> <span data-ttu-id="32d3f-157">Om reservationens användning är mellan 1 % och 99 % finns det oanvända fördelar.</span><span class="sxs-lookup"><span data-stu-id="32d3f-157">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="32d3f-158">Du kan undvika den här situationen genom att fastställa rätt storlek på den virtuella datorn för att stödja kundens databehandlingsbehov innan du gör köpet.</span><span class="sxs-lookup"><span data-stu-id="32d3f-158">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="32d3f-159">Verifiera kundens reservationsanvändning med API:et för Azure-användning</span><span class="sxs-lookup"><span data-stu-id="32d3f-159">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="32d3f-160">Endast API:et för Azure-användning visar vilken virtuell dator rabatten tillämpas på.</span><span class="sxs-lookup"><span data-stu-id="32d3f-160">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="32d3f-161">Du kan hämta reservationsanvändningsdata med API:et för Azure-användning för att verifiera att kunden får reservationsrabatten och för att se vilka virtuella datorer (virtuella datorer) som rabatten tillämpas på.</span><span class="sxs-lookup"><span data-stu-id="32d3f-161">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="32d3f-162">Jämför exempel A med exempel B för att se hur du verifierar en kunds reservationsanvändning.</span><span class="sxs-lookup"><span data-stu-id="32d3f-162">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Exempel på reservationsanvändning.":::

- <span data-ttu-id="32d3f-164">reservationId identifierar den Azure-reservation som användes för att tillämpa rabatten på den virtuella datorn.</span><span class="sxs-lookup"><span data-stu-id="32d3f-164">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="32d3f-165">consumptionMeter är MeterId för den virtuella dator där reservationsrabatten tillämpas.</span><span class="sxs-lookup"><span data-stu-id="32d3f-165">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="32d3f-166">ReservationMeter visar en kostnad på 0 USD sedan reservationsrabatten tillämpades.</span><span class="sxs-lookup"><span data-stu-id="32d3f-166">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="32d3f-167">Mer information finns i [Hämta en kunds användningsposter för Azure i](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) Partner Center [API.](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="32d3f-167">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="32d3f-168">Programvarukostnader, till exempel Microsoft Windows Server, ingår för närvarande inte i priset för en VM-reservation och visas som separata radobjekt i orderposten och på din faktura.</span><span class="sxs-lookup"><span data-stu-id="32d3f-168">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="32d3f-169">Men om en kund har Azure Hybrid-förmånen tillämpas inte programvarukostnaderna.</span><span class="sxs-lookup"><span data-stu-id="32d3f-169">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="32d3f-170">Mer information finns i Windows [programvarukostnader som inte ingår i reserverade instanser.](/azure/billing/billing-reserved-instance-windows-software-costs)</span><span class="sxs-lookup"><span data-stu-id="32d3f-170">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="32d3f-171">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="32d3f-171">Next steps</span></span>

|<span data-ttu-id="32d3f-172">**För information om**</span><span class="sxs-lookup"><span data-stu-id="32d3f-172">**For information about**</span></span>   |<span data-ttu-id="32d3f-173">**Läs detta**</span><span class="sxs-lookup"><span data-stu-id="32d3f-173">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="32d3f-174">Översikt över Azure-reservationer i CSP</span><span class="sxs-lookup"><span data-stu-id="32d3f-174">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="32d3f-175">Sälja Microsoft Azure reserverade VM-instanser</span><span class="sxs-lookup"><span data-stu-id="32d3f-175">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="32d3f-176">Köpa Azure-reservationer för dina kunder i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="32d3f-176">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="32d3f-177">Köpa Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="32d3f-177">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="32d3f-178">Hantera Azure-reservationer i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="32d3f-178">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="32d3f-179">Hantera Azure-reservationer i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="32d3f-179">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="32d3f-180">Köpa Azure-reservationer i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="32d3f-180">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="32d3f-181">[Förskottsbetala för virtuella datorer Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) i Azure-hjälpen</span><span class="sxs-lookup"><span data-stu-id="32d3f-181">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="32d3f-182">Hantera Azure-reservationer i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="32d3f-182">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="32d3f-183">[Hantera reserverade VM-instanser](/azure/billing/billing-manage-reserved-vm-instance) i Azure-hjälpen</span><span class="sxs-lookup"><span data-stu-id="32d3f-183">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="32d3f-184">Köpa Azure-reservationer med partnercenter-API:et</span><span class="sxs-lookup"><span data-stu-id="32d3f-184">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="32d3f-185">[Köp Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) i utvecklardokumentationen för Partnercenter</span><span class="sxs-lookup"><span data-stu-id="32d3f-185">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="32d3f-186">Ge kunderna tillstånd att köpa sina egna Azure-reservationer från en prenumeration som du har köpt åt dem.</span><span class="sxs-lookup"><span data-stu-id="32d3f-186">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="32d3f-187">Ge kunderna behörighet att köpa sina egna Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="32d3f-187">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |