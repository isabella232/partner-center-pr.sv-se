---
title: Effektiv enhetsprisberäkning
ms.topic: how-to
ms.date: 04/02/2021
description: Lär dig mer om det effektiva enhetspriset och hur det beräknas. Den här artikeln innehåller även en exempelberäkning.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6c3c3a672de015c9f38fa0e34232da8d9913177c
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528565"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="5658f-104">Effektiv enhetsprisberäkning för Förbrukning i Azure-plan</span><span class="sxs-lookup"><span data-stu-id="5658f-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="5658f-105">Det effektiva enhetspriset</span><span class="sxs-lookup"><span data-stu-id="5658f-105">The effective unit price</span></span>

<span data-ttu-id="5658f-106">Det effektiva enhetspriset beräknas på mätarnivå (till skillnad från resursnivån) och justeras dagligen enligt mätaranvändningen.</span><span class="sxs-lookup"><span data-stu-id="5658f-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="5658f-107">Vi beräknar det effektiva enhetspriset med hjälp av följande tre faktorer:</span><span class="sxs-lookup"><span data-stu-id="5658f-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="5658f-108">Förbrukning, som övervakas dagligen under faktureringsperioden</span><span class="sxs-lookup"><span data-stu-id="5658f-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="5658f-109">Fakturerbar kostnad för mätaren</span><span class="sxs-lookup"><span data-stu-id="5658f-109">Billable cost for the meter</span></span>
- <span data-ttu-id="5658f-110">Nivåindelad (om tillämpligt)</span><span class="sxs-lookup"><span data-stu-id="5658f-110">Tiering (if applicable)</span></span>

<span data-ttu-id="5658f-111">Eftersom vi övervakar förbrukningen varje dag under faktureringsperioden varierar det effektiva enhetspriset.</span><span class="sxs-lookup"><span data-stu-id="5658f-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="5658f-112">Det slutliga priset för en viss faktureringsperiod blir tillgängligt när vi stoppar förbrukningsberäkningen och stänger faktureringsperioden.</span><span class="sxs-lookup"><span data-stu-id="5658f-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="5658f-113">Du ser de flesta förbrukningsändringarna efter den fjärde eller femte decimalen.</span><span class="sxs-lookup"><span data-stu-id="5658f-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="5658f-114">Ta reda på om din mätare använder nivåindelade priser</span><span class="sxs-lookup"><span data-stu-id="5658f-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="5658f-115">Om du inte vet om mätaren använder nivåindelad prissättning kan du använda proceduren nedan för att ta reda på det.</span><span class="sxs-lookup"><span data-stu-id="5658f-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="5658f-116">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="5658f-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="5658f-117">Välj **Sälj,** välj **Priser och erbjudanden** och välj sedan Priser för **Azure-plan.**</span><span class="sxs-lookup"><span data-stu-id="5658f-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="5658f-118">Leta upp din mätare efter ID och ladda sedan ned dina prisdata.</span><span class="sxs-lookup"><span data-stu-id="5658f-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="5658f-119">Exempelberäkning</span><span class="sxs-lookup"><span data-stu-id="5658f-119">Sample calculation</span></span>

<span data-ttu-id="5658f-120">Tabellen nedan ger ett exempel på hur vi beräknar det effektiva enhetspriset under den öppna perioden.</span><span class="sxs-lookup"><span data-stu-id="5658f-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="5658f-121">I tabellen gäller följande värden:</span><span class="sxs-lookup"><span data-stu-id="5658f-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="5658f-122">**UP** = Enhetspris för resursen/timmen = 0,868</span><span class="sxs-lookup"><span data-stu-id="5658f-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="5658f-123">**BCU** = Fakturerbar förbrukningsenhet för mätaren</span><span class="sxs-lookup"><span data-stu-id="5658f-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="5658f-124">**BC** = Fakturerbar kostnad för mätaren = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="5658f-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="5658f-125">Detta återspeglar en justering för 15 % PEC-rabatten.</span><span class="sxs-lookup"><span data-stu-id="5658f-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="5658f-126">Sedan använder vi den nedre gränsen för funktionen för att begränsa värdet till två siffror efter decimaltecknet för att debitera det minsta beloppet.</span><span class="sxs-lookup"><span data-stu-id="5658f-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="5658f-127">**Gällande enhetspris** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="5658f-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="5658f-128">Obs! Mätaren i det här exemplet har inga prisnivåer eller andra rabatter – de effektiva enhetsprisfaktorerna i rabattprocent och andra justeringar.</span><span class="sxs-lookup"><span data-stu-id="5658f-128">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="5658f-129">Datum</span><span class="sxs-lookup"><span data-stu-id="5658f-129">Date</span></span> | <span data-ttu-id="5658f-130">BCU (fakturerbar förbrukningsenhet)</span><span class="sxs-lookup"><span data-stu-id="5658f-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="5658f-131">BC (fakturerbar kostnad)</span><span class="sxs-lookup"><span data-stu-id="5658f-131">BC (Billable cost)</span></span> | <span data-ttu-id="5658f-132">Effektivt enhetspris</span><span class="sxs-lookup"><span data-stu-id="5658f-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="5658f-133">3 augusti</span><span class="sxs-lookup"><span data-stu-id="5658f-133">3-Aug</span></span> | <span data-ttu-id="5658f-134">29</span><span class="sxs-lookup"><span data-stu-id="5658f-134">29</span></span> | <span data-ttu-id="5658f-135">21.39</span><span class="sxs-lookup"><span data-stu-id="5658f-135">21.39</span></span> | <span data-ttu-id="5658f-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="5658f-136">0.737586206896552</span></span> |
| <span data-ttu-id="5658f-137">10 augusti</span><span class="sxs-lookup"><span data-stu-id="5658f-137">10-Aug</span></span> | <span data-ttu-id="5658f-138">210.950039</span><span class="sxs-lookup"><span data-stu-id="5658f-138">210.950039</span></span> | <span data-ttu-id="5658f-139">155.63</span><span class="sxs-lookup"><span data-stu-id="5658f-139">155.63</span></span> | <span data-ttu-id="5658f-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="5658f-140">0.737757626107858</span></span> |
| <span data-ttu-id="5658f-141">25 augusti</span><span class="sxs-lookup"><span data-stu-id="5658f-141">25-Aug</span></span> | <span data-ttu-id="5658f-142">555.950039</span><span class="sxs-lookup"><span data-stu-id="5658f-142">555.950039</span></span> | <span data-ttu-id="5658f-143">410.17</span><span class="sxs-lookup"><span data-stu-id="5658f-143">410.17</span></span> | <span data-ttu-id="5658f-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="5658f-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="5658f-145">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="5658f-145">Next steps</span></span>

- [<span data-ttu-id="5658f-146">Fakturering och skatter</span><span class="sxs-lookup"><span data-stu-id="5658f-146">Billing and taxes</span></span>](billing.md)
