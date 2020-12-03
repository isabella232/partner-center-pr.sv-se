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
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="35ca6-103">Storleksändring av virtuell Microsoft Azure-dator för maximal reservationsanvändning</span><span class="sxs-lookup"><span data-stu-id="35ca6-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="35ca6-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="35ca6-104">**Appropriate roles**</span></span>

- <span data-ttu-id="35ca6-105">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="35ca6-105">Admin agent</span></span>
- <span data-ttu-id="35ca6-106">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="35ca6-106">Sales agent</span></span>

<span data-ttu-id="35ca6-107">Den här artikeln förklarar hur du ändrar storlek på en virtuell dator (VM) till dina kunders behov när du köper Microsoft Azure reservationer för dem.</span><span class="sxs-lookup"><span data-stu-id="35ca6-107">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="35ca6-108">Den här artikeln gäller endast partner i Cloud Solution Provider (CSP)-programmet.</span><span class="sxs-lookup"><span data-stu-id="35ca6-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="35ca6-109">Kunder som använder andra typer av prenumerationer (t. ex. betala per användning, enskilda, Microsoft-kundavtal eller Enterprise-avtal prenumerationer) bör i stället läsa [denna dokumentation om Azure-reservationer](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="35ca6-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="35ca6-110">Fastställa storleken på den virtuella datorn för en kunds Azure-reservation</span><span class="sxs-lookup"><span data-stu-id="35ca6-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="35ca6-111">När du köper Microsoft Azure reservationer för dina kunders räkning måste du välja en storlek för virtuella datorer (VM) för att uppfylla kundens data bearbetnings behov.</span><span class="sxs-lookup"><span data-stu-id="35ca6-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="35ca6-112">Du kan hitta den här informationen på något av följande sätt:</span><span class="sxs-lookup"><span data-stu-id="35ca6-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="35ca6-113">API för Azure-användning</span><span class="sxs-lookup"><span data-stu-id="35ca6-113">Azure utilization API</span></span>
- <span data-ttu-id="35ca6-114">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="35ca6-114">The Azure portal</span></span>
- <span data-ttu-id="35ca6-115">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="35ca6-115">Azure PowerShell</span></span>
- <span data-ttu-id="35ca6-116">API för Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="35ca6-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="35ca6-117">Instruktioner för att använda var och en av dessa metoder finns nedan.</span><span class="sxs-lookup"><span data-stu-id="35ca6-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="35ca6-118">När du har köpt en reservation tillämpas reservations rabatten automatiskt på virtuella datorer som matchar attributen och mängden av reservationen.</span><span class="sxs-lookup"><span data-stu-id="35ca6-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="35ca6-119">Du behöver inte tilldela reservationen till en virtuell dator.</span><span class="sxs-lookup"><span data-stu-id="35ca6-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="35ca6-120">Reservations rabatter gäller inte för klassiska virtuella datorer eller reklam.</span><span class="sxs-lookup"><span data-stu-id="35ca6-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="35ca6-121">För att korrekt identifiera typen och storleken på den virtuella datorn som ska köpas åt kunden, måste du använda en av de metoder som beskrivs nedan eftersom typen av VM-serien inte visas korrekt i filer för partner av Partner Center.</span><span class="sxs-lookup"><span data-stu-id="35ca6-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="35ca6-122">Hämta storleks information för virtuella datorer med Azures användnings-API</span><span class="sxs-lookup"><span data-stu-id="35ca6-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="35ca6-123">Använd värdet för attributet ServiceType från additionalInfo i API-svaret för att identifiera den VM-storlek som ska köpas.</span><span class="sxs-lookup"><span data-stu-id="35ca6-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="35ca6-124">Mer information finns i [Hämta en kunds användnings poster för Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) i [partner Center API](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="35ca6-124">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="35ca6-125">Hämta storleks information för virtuella datorer med hjälp av Microsoft Azure-portalen</span><span class="sxs-lookup"><span data-stu-id="35ca6-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="35ca6-126">Gå till sidan **kunder** i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="35ca6-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="35ca6-127">Hitta kunden som vill köpa reservationer för virtuella Azure-datorer och välj sedan nedpilen för att expandera kundens information.</span><span class="sxs-lookup"><span data-stu-id="35ca6-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="35ca6-128">Välj **Microsoft Azure-hanteringsportal** för att öppna kundens post i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="35ca6-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="35ca6-129">Välj **virtuella datorer** på Portal-menyn och välj sedan den virtuella dator som du vill köpa en reservation för.</span><span class="sxs-lookup"><span data-stu-id="35ca6-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="35ca6-130">På sidan information om den virtuella datorn hittar du storlek och regions information, enligt nedan, och använder den här informationen för att köpa reservationen i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="35ca6-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Storlek och regions information på informations Sidan":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="35ca6-132">Hämta storleks information för virtuella datorer med Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="35ca6-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="35ca6-133">Använd informationen i bilden nedan för att hämta platsen och storleken på den virtuella dator som du vill köpa en reservation för.</span><span class="sxs-lookup"><span data-stu-id="35ca6-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM-plats och storlek":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="35ca6-135">Hämta storleks information för virtuella datorer med hjälp av API: et för Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="35ca6-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="35ca6-136">Använd ARMClient eller ARM-API: erna för att anropa ARM-klienten för den virtuella dator som du vill köpa en reservation för.</span><span class="sxs-lookup"><span data-stu-id="35ca6-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="35ca6-137">/Subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="35ca6-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="35ca6-138">Anropet returnerar värdena för **vmSize** och **platsen**, enligt nedan.</span><span class="sxs-lookup"><span data-stu-id="35ca6-138">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize-värde":::
    :::image type="content" source="images/usage4.png" alt-text="plats värde":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="35ca6-141">Verifiera användningen av virtuella Azure-datorer och reservations rabatt</span><span class="sxs-lookup"><span data-stu-id="35ca6-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="35ca6-142">När du har köpt en Azure reserverad VM-instans för en kunds räkning, tillämpas rabatten för att betala för VM-utrymme i förväg automatiskt på de virtuella datorer som matchar attributen och antalet för kundens reservation.</span><span class="sxs-lookup"><span data-stu-id="35ca6-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="35ca6-143">Du kan kontrol lera kundens reservations användning och se vilka virtuella datorer som reservations rabatterna tillämpas på med hjälp av någon av följande metoder:</span><span class="sxs-lookup"><span data-stu-id="35ca6-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="35ca6-144">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="35ca6-144">The Azure portal</span></span>
- <span data-ttu-id="35ca6-145">API för Azure-användning</span><span class="sxs-lookup"><span data-stu-id="35ca6-145">Azure utilization API</span></span>

<span data-ttu-id="35ca6-146">Instruktioner för att använda var och en av dessa metoder finns nedan.</span><span class="sxs-lookup"><span data-stu-id="35ca6-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="35ca6-147">Endast Azures användnings-API: et visar vilken virtuell dator som rabatten tillämpas på.</span><span class="sxs-lookup"><span data-stu-id="35ca6-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="35ca6-148">Verifiera kundens reservations användning i Microsoft Azure-portalen</span><span class="sxs-lookup"><span data-stu-id="35ca6-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="35ca6-149">Gå till sidan **kunder** i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="35ca6-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="35ca6-150">Hitta kunden vars reservations rabatt och användning du vill verifiera och välj sedan nedpilen för att expandera kundens information.</span><span class="sxs-lookup"><span data-stu-id="35ca6-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="35ca6-151">Välj **Microsoft Azure-hanteringsportal** för att öppna kundens post i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="35ca6-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="35ca6-152">Välj **reservationer** på Portal-menyn och välj sedan den reservation som du vill kontrol lera användningen för.</span><span class="sxs-lookup"><span data-stu-id="35ca6-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="35ca6-153">På sidan **Översikt** kontrollerar du diagrammets användnings diagram för reservationen, som visar hur mycket av reservationen som tillämpades på virtuella datorer.</span><span class="sxs-lookup"><span data-stu-id="35ca6-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="35ca6-154">Användnings data kan fördröjas med upp till 8 timmar.</span><span class="sxs-lookup"><span data-stu-id="35ca6-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="35ca6-155">a.</span><span class="sxs-lookup"><span data-stu-id="35ca6-155">a.</span></span> <span data-ttu-id="35ca6-156">Om reservationens användning är 100% får kunden alla tänkbara besparingar som kan tillhandahållas av reservations köpet.</span><span class="sxs-lookup"><span data-stu-id="35ca6-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="35ca6-157">b.</span><span class="sxs-lookup"><span data-stu-id="35ca6-157">b.</span></span> <span data-ttu-id="35ca6-158">Om reservationens användning är 0% används inte rabatten på någon virtuell dator.</span><span class="sxs-lookup"><span data-stu-id="35ca6-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="35ca6-159">c.</span><span class="sxs-lookup"><span data-stu-id="35ca6-159">c.</span></span> <span data-ttu-id="35ca6-160">Om reservationens användning är mellan 1% och 99%, finns det några outnyttjade förmåner.</span><span class="sxs-lookup"><span data-stu-id="35ca6-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="35ca6-161">Undvik den här situationen genom att fastställa rätt storlek på den virtuella datorn som stöder kundens dator behov innan du gör köpet.</span><span class="sxs-lookup"><span data-stu-id="35ca6-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="35ca6-162">Verifiera kundens reservations användning med Azures API för användning</span><span class="sxs-lookup"><span data-stu-id="35ca6-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="35ca6-163">Endast Azures användnings-API: et visar vilken virtuell dator som rabatten tillämpas på.</span><span class="sxs-lookup"><span data-stu-id="35ca6-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="35ca6-164">Du kan hämta reservations användnings data med Azure Usage API för att kontrol lera att kunden får reservations rabatten och se vilka virtuella datorer (virtuella datorer) som rabatten tillämpas på.</span><span class="sxs-lookup"><span data-stu-id="35ca6-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="35ca6-165">Jämför exempel A till exempel B för att se hur du verifierar en kunds reservations användning.</span><span class="sxs-lookup"><span data-stu-id="35ca6-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Exempel på reservations användning":::

- <span data-ttu-id="35ca6-167">ReservationId identifierar den Azure-reservation som användes för att tillämpa rabatten på den virtuella datorn.</span><span class="sxs-lookup"><span data-stu-id="35ca6-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="35ca6-168">consumptionMeter är MeterId för den virtuella dator som har reservations rabatten som tillämpas.</span><span class="sxs-lookup"><span data-stu-id="35ca6-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="35ca6-169">ReservationMeter visar $0-kostnaden sedan reservations Rabatten tillämpades.</span><span class="sxs-lookup"><span data-stu-id="35ca6-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="35ca6-170">Mer information finns i [Hämta en kunds användnings poster för Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) i [partner Center API](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="35ca6-170">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="35ca6-171">Program varu kostnader, till exempel Microsoft Windows Server, ingår för närvarande inte i priset för en VM-reservation och visas som separata rad objekt i order posten och på din faktura.</span><span class="sxs-lookup"><span data-stu-id="35ca6-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="35ca6-172">Men om en kund har Azure Hybrid Use-förmånen kommer program kostnaden inte att tillämpas.</span><span class="sxs-lookup"><span data-stu-id="35ca6-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="35ca6-173">Mer information finns i [Windows-programkostnader som inte ingår i reserverade instanser](/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="35ca6-173">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="35ca6-174">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="35ca6-174">Next steps</span></span>

|<span data-ttu-id="35ca6-175">**För information om**</span><span class="sxs-lookup"><span data-stu-id="35ca6-175">**For information about**</span></span>   |<span data-ttu-id="35ca6-176">**Läs detta**</span><span class="sxs-lookup"><span data-stu-id="35ca6-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="35ca6-177">Översikt över Azure-reservationer i CSP</span><span class="sxs-lookup"><span data-stu-id="35ca6-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="35ca6-178">Sälj Microsoft Azure reserverade VM-instanser</span><span class="sxs-lookup"><span data-stu-id="35ca6-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="35ca6-179">Köpa Azure-reservationer för dina kunder i Partner Center</span><span class="sxs-lookup"><span data-stu-id="35ca6-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="35ca6-180">Köp Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="35ca6-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="35ca6-181">Hantera Azure-reservationer i Partner Center</span><span class="sxs-lookup"><span data-stu-id="35ca6-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="35ca6-182">Hantera Azure-reservationer i Partner Center</span><span class="sxs-lookup"><span data-stu-id="35ca6-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="35ca6-183">Köpa Azure-reservationer i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="35ca6-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="35ca6-184">[Förskotts betalning för virtuella datorer med Azure Reserved VM instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) i Azure-hjälpen</span><span class="sxs-lookup"><span data-stu-id="35ca6-184">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="35ca6-185">Hantera Azure-reservationer i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="35ca6-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="35ca6-186">[Hantera reserverade VM-instanser](/azure/billing/billing-manage-reserved-vm-instance) i Azure-hjälpen</span><span class="sxs-lookup"><span data-stu-id="35ca6-186">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="35ca6-187">Köpa Azure-reservationer med partner Center API</span><span class="sxs-lookup"><span data-stu-id="35ca6-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="35ca6-188">[Köp Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) i dokumentationen för partner Center-utvecklare</span><span class="sxs-lookup"><span data-stu-id="35ca6-188">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="35ca6-189">Ge kunderna tillstånd att köpa sina egna Azure-reservationer från en prenumeration som du har köpt för dem.</span><span class="sxs-lookup"><span data-stu-id="35ca6-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="35ca6-190">Ge kunderna tillstånd att köpa sina egna Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="35ca6-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |