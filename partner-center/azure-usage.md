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
ms.openlocfilehash: e6c4e3e7a68de720f586754703308a447d7d30c1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531621"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="56a24-103">Storleksändring av virtuell Microsoft Azure-dator för maximal reservationsanvändning</span><span class="sxs-lookup"><span data-stu-id="56a24-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="56a24-104">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="56a24-104">**Applies to**</span></span>

- <span data-ttu-id="56a24-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="56a24-105">Partner Center</span></span>
- <span data-ttu-id="56a24-106">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="56a24-106">Azure portal</span></span>
- <span data-ttu-id="56a24-107">Partner i CSP-programmet</span><span class="sxs-lookup"><span data-stu-id="56a24-107">Partners in the CSP program</span></span>
 
> [!NOTE]
> <span data-ttu-id="56a24-108">Den här artikeln gäller endast partner i Cloud Solution Provider (CSP)-programmet.</span><span class="sxs-lookup"><span data-stu-id="56a24-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="56a24-109">Kunder som använder andra typer av prenumerationer (t. ex. betala per användning, enskilda, Microsoft-kundavtal eller Enterprise-avtal prenumerationer) bör i stället läsa [denna dokumentation om Azure-reservationer](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="56a24-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="56a24-110">Fastställa storleken på den virtuella datorn för en kunds Azure-reservation</span><span class="sxs-lookup"><span data-stu-id="56a24-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="56a24-111">När du köper Microsoft Azure reservationer för dina kunders räkning måste du välja en storlek för virtuella datorer (VM) för att uppfylla kundens data bearbetnings behov.</span><span class="sxs-lookup"><span data-stu-id="56a24-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="56a24-112">Du kan hitta den här informationen på något av följande sätt:</span><span class="sxs-lookup"><span data-stu-id="56a24-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="56a24-113">API för Azure-användning</span><span class="sxs-lookup"><span data-stu-id="56a24-113">Azure utilization API</span></span>
- <span data-ttu-id="56a24-114">Azure-portalen</span><span class="sxs-lookup"><span data-stu-id="56a24-114">The Azure portal</span></span>
- <span data-ttu-id="56a24-115">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="56a24-115">Azure PowerShell</span></span>
- <span data-ttu-id="56a24-116">API för Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="56a24-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="56a24-117">Instruktioner för att använda var och en av dessa metoder finns nedan.</span><span class="sxs-lookup"><span data-stu-id="56a24-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="56a24-118">När du har köpt en reservation tillämpas reservations rabatten automatiskt på virtuella datorer som matchar attributen och mängden av reservationen.</span><span class="sxs-lookup"><span data-stu-id="56a24-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="56a24-119">Du behöver inte tilldela reservationen till en virtuell dator.</span><span class="sxs-lookup"><span data-stu-id="56a24-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="56a24-120">Reservations rabatter gäller inte för klassiska virtuella datorer eller reklam.</span><span class="sxs-lookup"><span data-stu-id="56a24-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="56a24-121">För att korrekt identifiera typen och storleken på den virtuella datorn som ska köpas åt kunden, måste du använda en av de metoder som beskrivs nedan eftersom typen av VM-serien inte visas korrekt i filer för partner av Partner Center.</span><span class="sxs-lookup"><span data-stu-id="56a24-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="56a24-122">Hämta storleks information för virtuella datorer med Azures användnings-API</span><span class="sxs-lookup"><span data-stu-id="56a24-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="56a24-123">Använd värdet för attributet ServiceType från additionalInfo i API-svaret för att identifiera den VM-storlek som ska köpas.</span><span class="sxs-lookup"><span data-stu-id="56a24-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="56a24-124">Mer information finns i [Hämta en kunds användnings poster för Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) i [partner Center API](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="56a24-124">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="56a24-125">Hämta storleks information för virtuella datorer med hjälp av Microsoft Azure-portalen</span><span class="sxs-lookup"><span data-stu-id="56a24-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="56a24-126">Gå till sidan **kunder** i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="56a24-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="56a24-127">Hitta kunden som vill köpa reservationer för virtuella Azure-datorer och välj sedan nedpilen för att expandera kundens information.</span><span class="sxs-lookup"><span data-stu-id="56a24-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="56a24-128">Välj **Microsoft Azure-hanteringsportal** för att öppna kundens post i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="56a24-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="56a24-129">Välj **virtuella datorer** på Portal-menyn och välj sedan den virtuella dator som du vill köpa en reservation för.</span><span class="sxs-lookup"><span data-stu-id="56a24-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="56a24-130">På sidan information om den virtuella datorn hittar du storlek och regions information, enligt nedan, och använder den här informationen för att köpa reservationen i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="56a24-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Storlek och regions information på informations Sidan":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="56a24-132">Hämta storleks information för virtuella datorer med Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="56a24-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="56a24-133">Använd informationen i bilden nedan för att hämta platsen och storleken på den virtuella dator som du vill köpa en reservation för.</span><span class="sxs-lookup"><span data-stu-id="56a24-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM-plats och storlek":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="56a24-135">Hämta storleks information för virtuella datorer med hjälp av API: et för Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="56a24-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="56a24-136">Använd ARMClient eller ARM-API: erna för att anropa ARM-klienten för den virtuella dator som du vill köpa en reservation för.</span><span class="sxs-lookup"><span data-stu-id="56a24-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="56a24-137">/Subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="56a24-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="56a24-138">Anropet returnerar värdena för **vmSize** och **platsen** , enligt nedan.</span><span class="sxs-lookup"><span data-stu-id="56a24-138">The call returns the values for **vmSize** and **location** , as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize-värde":::
    :::image type="content" source="images/usage4.png" alt-text="plats värde":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="56a24-141">Verifiera användningen av virtuella Azure-datorer och reservations rabatt</span><span class="sxs-lookup"><span data-stu-id="56a24-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="56a24-142">När du har köpt en Azure reserverad VM-instans för en kunds räkning, tillämpas rabatten för att betala för VM-utrymme i förväg automatiskt på de virtuella datorer som matchar attributen och antalet för kundens reservation.</span><span class="sxs-lookup"><span data-stu-id="56a24-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="56a24-143">Du kan kontrol lera kundens reservations användning och se vilka virtuella datorer som reservations rabatterna tillämpas på med hjälp av någon av följande metoder:</span><span class="sxs-lookup"><span data-stu-id="56a24-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="56a24-144">Azure-portalen</span><span class="sxs-lookup"><span data-stu-id="56a24-144">The Azure portal</span></span>
- <span data-ttu-id="56a24-145">API för Azure-användning</span><span class="sxs-lookup"><span data-stu-id="56a24-145">Azure utilization API</span></span>

<span data-ttu-id="56a24-146">Instruktioner för att använda var och en av dessa metoder finns nedan.</span><span class="sxs-lookup"><span data-stu-id="56a24-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="56a24-147">Endast Azures användnings-API: et visar vilken virtuell dator som rabatten tillämpas på.</span><span class="sxs-lookup"><span data-stu-id="56a24-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="56a24-148">Verifiera kundens reservations användning i Microsoft Azure-portalen</span><span class="sxs-lookup"><span data-stu-id="56a24-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="56a24-149">Gå till sidan **kunder** i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="56a24-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="56a24-150">Hitta kunden vars reservations rabatt och användning du vill verifiera och välj sedan nedpilen för att expandera kundens information.</span><span class="sxs-lookup"><span data-stu-id="56a24-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="56a24-151">Välj **Microsoft Azure-hanteringsportal** för att öppna kundens post i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="56a24-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="56a24-152">Välj **reservationer** på Portal-menyn och välj sedan den reservation som du vill kontrol lera användningen för.</span><span class="sxs-lookup"><span data-stu-id="56a24-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="56a24-153">På sidan **Översikt** kontrollerar du diagrammets användnings diagram för reservationen, som visar hur mycket av reservationen som tillämpades på virtuella datorer.</span><span class="sxs-lookup"><span data-stu-id="56a24-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="56a24-154">Användnings data kan fördröjas med upp till 8 timmar.</span><span class="sxs-lookup"><span data-stu-id="56a24-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="56a24-155">a.</span><span class="sxs-lookup"><span data-stu-id="56a24-155">a.</span></span> <span data-ttu-id="56a24-156">Om reservationens användning är 100% får kunden alla tänkbara besparingar som kan tillhandahållas av reservations köpet.</span><span class="sxs-lookup"><span data-stu-id="56a24-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="56a24-157">b.</span><span class="sxs-lookup"><span data-stu-id="56a24-157">b.</span></span> <span data-ttu-id="56a24-158">Om reservationens användning är 0% används inte rabatten på någon virtuell dator.</span><span class="sxs-lookup"><span data-stu-id="56a24-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="56a24-159">c.</span><span class="sxs-lookup"><span data-stu-id="56a24-159">c.</span></span> <span data-ttu-id="56a24-160">Om reservationens användning är mellan 1% och 99%, finns det några outnyttjade förmåner.</span><span class="sxs-lookup"><span data-stu-id="56a24-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="56a24-161">Undvik den här situationen genom att fastställa rätt storlek på den virtuella datorn som stöder kundens dator behov innan du gör köpet.</span><span class="sxs-lookup"><span data-stu-id="56a24-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="56a24-162">Verifiera kundens reservations användning med Azures API för användning</span><span class="sxs-lookup"><span data-stu-id="56a24-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="56a24-163">Endast Azures användnings-API: et visar vilken virtuell dator som rabatten tillämpas på.</span><span class="sxs-lookup"><span data-stu-id="56a24-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="56a24-164">Du kan hämta reservations användnings data med Azure Usage API för att kontrol lera att kunden får reservations rabatten och se vilka virtuella datorer (virtuella datorer) som rabatten tillämpas på.</span><span class="sxs-lookup"><span data-stu-id="56a24-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="56a24-165">Jämför exempel A till exempel B för att se hur du verifierar en kunds reservations användning.</span><span class="sxs-lookup"><span data-stu-id="56a24-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Exempel på reservations användning":::

- <span data-ttu-id="56a24-167">ReservationId identifierar den Azure-reservation som användes för att tillämpa rabatten på den virtuella datorn.</span><span class="sxs-lookup"><span data-stu-id="56a24-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="56a24-168">consumptionMeter är MeterId för den virtuella dator som har reservations rabatten som tillämpas.</span><span class="sxs-lookup"><span data-stu-id="56a24-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="56a24-169">ReservationMeter visar $0-kostnaden sedan reservations Rabatten tillämpades.</span><span class="sxs-lookup"><span data-stu-id="56a24-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="56a24-170">Mer information finns i [Hämta en kunds användnings poster för Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) i [partner Center API](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="56a24-170">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="56a24-171">Program varu kostnader, till exempel Microsoft Windows Server, ingår för närvarande inte i priset för en VM-reservation och visas som separata rad objekt i order posten och på din faktura.</span><span class="sxs-lookup"><span data-stu-id="56a24-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="56a24-172">Men om en kund har Azure Hybrid Use-förmånen kommer program kostnaden inte att tillämpas.</span><span class="sxs-lookup"><span data-stu-id="56a24-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="56a24-173">Mer information finns i [Windows-programkostnader som inte ingår i reserverade instanser](/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="56a24-173">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="56a24-174">Resurser för Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="56a24-174">Azure reservations resources</span></span>

|<span data-ttu-id="56a24-175">**För information om**</span><span class="sxs-lookup"><span data-stu-id="56a24-175">**For information about**</span></span>   |<span data-ttu-id="56a24-176">**Läs detta**</span><span class="sxs-lookup"><span data-stu-id="56a24-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="56a24-177">Översikt över Azure-reservationer i CSP</span><span class="sxs-lookup"><span data-stu-id="56a24-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="56a24-178">Sälj Microsoft Azure reserverade VM-instanser</span><span class="sxs-lookup"><span data-stu-id="56a24-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="56a24-179">Köpa Azure-reservationer för dina kunder i Partner Center</span><span class="sxs-lookup"><span data-stu-id="56a24-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="56a24-180">Köp Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="56a24-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="56a24-181">Hantera Azure-reservationer i Partner Center</span><span class="sxs-lookup"><span data-stu-id="56a24-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="56a24-182">Hantera Azure-reservationer i Partner Center</span><span class="sxs-lookup"><span data-stu-id="56a24-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="56a24-183">Köpa Azure-reservationer i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="56a24-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="56a24-184">[Förskotts betalning för virtuella datorer med Azure Reserved VM instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) i Azure-hjälpen</span><span class="sxs-lookup"><span data-stu-id="56a24-184">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="56a24-185">Hantera Azure-reservationer i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="56a24-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="56a24-186">[Hantera reserverade VM-instanser](/azure/billing/billing-manage-reserved-vm-instance) i Azure-hjälpen</span><span class="sxs-lookup"><span data-stu-id="56a24-186">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="56a24-187">Köpa Azure-reservationer med partner Center API</span><span class="sxs-lookup"><span data-stu-id="56a24-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="56a24-188">[Köp Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) i dokumentationen för partner Center-utvecklare</span><span class="sxs-lookup"><span data-stu-id="56a24-188">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="56a24-189">Ge kunderna tillstånd att köpa sina egna Azure-reservationer från en prenumeration som du har köpt för dem.</span><span class="sxs-lookup"><span data-stu-id="56a24-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="56a24-190">Ge kunderna tillstånd att köpa sina egna Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="56a24-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |