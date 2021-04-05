---
title: Effektiv enhetsprisberäkning
ms.topic: how-to
ms.date: 04/02/2021
description: Läs om det effektiva enhets priset och hur det beräknas. Den här artikeln innehåller även en exempel beräkning.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a662e0b815c979b3454762c5b35eb510887c96ad
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374406"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="1b525-104">Effektiv enhets pris beräkning för Azure plan-förbrukning</span><span class="sxs-lookup"><span data-stu-id="1b525-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="1b525-105">Det effektiva enhets priset</span><span class="sxs-lookup"><span data-stu-id="1b525-105">The effective unit price</span></span>

<span data-ttu-id="1b525-106">Det effektiva enhets priset beräknas på mätar nivån (till skillnad från resurs nivån) och justeras dagligen enligt mätnings användningen.</span><span class="sxs-lookup"><span data-stu-id="1b525-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="1b525-107">Vi beräknar det effektiva enhets priset med följande tre faktorer:</span><span class="sxs-lookup"><span data-stu-id="1b525-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="1b525-108">Förbrukning, som övervakas dagligen under fakturerings perioden</span><span class="sxs-lookup"><span data-stu-id="1b525-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="1b525-109">Fakturerbar kostnad för mätaren</span><span class="sxs-lookup"><span data-stu-id="1b525-109">Billable cost for the meter</span></span>
- <span data-ttu-id="1b525-110">Skiktning (om tillämpligt)</span><span class="sxs-lookup"><span data-stu-id="1b525-110">Tiering (if applicable)</span></span>

<span data-ttu-id="1b525-111">Eftersom vi övervakar förbrukning dagligen under hela fakturerings perioden kommer det effektiva enhets priset att variera.</span><span class="sxs-lookup"><span data-stu-id="1b525-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="1b525-112">Det slutgiltiga priset för en viss fakturerings cykel blir tillgängligt efter att du har stoppat förbruknings beräkningen och stängt fakturerings perioden.</span><span class="sxs-lookup"><span data-stu-id="1b525-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="1b525-113">Du ser de flesta förändringar i förbrukningen efter den fjärde eller femte decimalen.</span><span class="sxs-lookup"><span data-stu-id="1b525-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="1b525-114">Ta reda på om din mätning använder nivå priser</span><span class="sxs-lookup"><span data-stu-id="1b525-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="1b525-115">Om du inte vet om mätaren använder nivå priser använder du proceduren nedan för att ta reda på det.</span><span class="sxs-lookup"><span data-stu-id="1b525-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="1b525-116">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="1b525-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="1b525-117">Välj **sälja**, Välj **priser och erbjudanden** och välj sedan **pris för Azure-prenumeration**.</span><span class="sxs-lookup"><span data-stu-id="1b525-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="1b525-118">Leta upp din mätning efter ID och ladda ned dina pris data.</span><span class="sxs-lookup"><span data-stu-id="1b525-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="1b525-119">Exempel beräkning</span><span class="sxs-lookup"><span data-stu-id="1b525-119">Sample calculation</span></span>

<span data-ttu-id="1b525-120">Tabellen nedan visar ett exempel på hur vi beräknar det effektiva enhets priset under den öppna perioden.</span><span class="sxs-lookup"><span data-stu-id="1b525-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="1b525-121">I tabellen gäller följande värden:</span><span class="sxs-lookup"><span data-stu-id="1b525-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="1b525-122">**Upp** = enhets priset för resursen/timmen = 0,868</span><span class="sxs-lookup"><span data-stu-id="1b525-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="1b525-123">**BCU** = fakturerbar förbruknings enhet för mätaren</span><span class="sxs-lookup"><span data-stu-id="1b525-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="1b525-124">**BC** = fakturerbar kostnad för mätaren = BCU \* upp \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="1b525-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="1b525-125">Detta motsvarar en justering för 15% PEC-rabatten.</span><span class="sxs-lookup"><span data-stu-id="1b525-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="1b525-126">Vi använder sedan den nedre gränsen för funktionen för att begränsa värdet till två siffror efter decimal tecknet, för att debitera minimi beloppet.</span><span class="sxs-lookup"><span data-stu-id="1b525-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="1b525-127">**Effektivt enhets pris** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="1b525-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="1b525-128">Mätaren i det här exemplet saknar nivåer i prissättningen.</span><span class="sxs-lookup"><span data-stu-id="1b525-128">The meter in this example does not have tiers in pricing.</span></span> <span data-ttu-id="1b525-129">De effektiva enhets pris faktorerna i rabatt procent och andra justeringar.</span><span class="sxs-lookup"><span data-stu-id="1b525-129">The Effective Unit Price factors in discount percentages and other adjustments.</span></span>

| <span data-ttu-id="1b525-130">Datum</span><span class="sxs-lookup"><span data-stu-id="1b525-130">Date</span></span> | <span data-ttu-id="1b525-131">BCU (fakturerbar förbruknings enhet)</span><span class="sxs-lookup"><span data-stu-id="1b525-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="1b525-132">BC (fakturerbar kostnad)</span><span class="sxs-lookup"><span data-stu-id="1b525-132">BC (Billable cost)</span></span> | <span data-ttu-id="1b525-133">Effektivt enhets pris</span><span class="sxs-lookup"><span data-stu-id="1b525-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="1b525-134">3 – aug</span><span class="sxs-lookup"><span data-stu-id="1b525-134">3-Aug</span></span> | <span data-ttu-id="1b525-135">29</span><span class="sxs-lookup"><span data-stu-id="1b525-135">29</span></span> | <span data-ttu-id="1b525-136">21,39</span><span class="sxs-lookup"><span data-stu-id="1b525-136">21.39</span></span> | <span data-ttu-id="1b525-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="1b525-137">0.737586206896552</span></span> |
| <span data-ttu-id="1b525-138">10 – aug</span><span class="sxs-lookup"><span data-stu-id="1b525-138">10-Aug</span></span> | <span data-ttu-id="1b525-139">210,950039</span><span class="sxs-lookup"><span data-stu-id="1b525-139">210.950039</span></span> | <span data-ttu-id="1b525-140">155,63</span><span class="sxs-lookup"><span data-stu-id="1b525-140">155.63</span></span> | <span data-ttu-id="1b525-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="1b525-141">0.737757626107858</span></span> |
| <span data-ttu-id="1b525-142">25 – aug</span><span class="sxs-lookup"><span data-stu-id="1b525-142">25-Aug</span></span> | <span data-ttu-id="1b525-143">555,950039</span><span class="sxs-lookup"><span data-stu-id="1b525-143">555.950039</span></span> | <span data-ttu-id="1b525-144">410,17</span><span class="sxs-lookup"><span data-stu-id="1b525-144">410.17</span></span> | <span data-ttu-id="1b525-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="1b525-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="1b525-146">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="1b525-146">Next steps</span></span>

- [<span data-ttu-id="1b525-147">Fakturering och skatter</span><span class="sxs-lookup"><span data-stu-id="1b525-147">Billing and taxes</span></span>](billing.md)
