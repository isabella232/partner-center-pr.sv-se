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
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172225"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="97c28-104">Effektiv enhetsprisberäkning för Förbrukning i Azure-plan</span><span class="sxs-lookup"><span data-stu-id="97c28-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="97c28-105">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="97c28-105">**Appropriate roles**</span></span>

- <span data-ttu-id="97c28-106">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="97c28-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="97c28-107">Det effektiva enhetspriset</span><span class="sxs-lookup"><span data-stu-id="97c28-107">The effective unit price</span></span>

<span data-ttu-id="97c28-108">Det effektiva enhetspriset beräknas på mätarnivå (till skillnad från resursnivån) och justeras dagligen enligt mätaranvändningen.</span><span class="sxs-lookup"><span data-stu-id="97c28-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="97c28-109">Vi beräknar det effektiva enhetspriset med hjälp av följande tre faktorer:</span><span class="sxs-lookup"><span data-stu-id="97c28-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="97c28-110">Förbrukning, som övervakas dagligen under faktureringsperioden</span><span class="sxs-lookup"><span data-stu-id="97c28-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="97c28-111">Fakturerbar kostnad för mätaren</span><span class="sxs-lookup"><span data-stu-id="97c28-111">Billable cost for the meter</span></span>
- <span data-ttu-id="97c28-112">Nivåindelad (om tillämpligt)</span><span class="sxs-lookup"><span data-stu-id="97c28-112">Tiering (if applicable)</span></span>

<span data-ttu-id="97c28-113">Eftersom vi övervakar förbrukningen varje dag under faktureringsperioden varierar det effektiva enhetspriset.</span><span class="sxs-lookup"><span data-stu-id="97c28-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="97c28-114">Det slutliga priset för en viss faktureringsperiod blir tillgängligt när vi stoppar förbrukningsberäkningen och stänger faktureringsperioden.</span><span class="sxs-lookup"><span data-stu-id="97c28-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="97c28-115">Du ser de flesta förbrukningsändringarna efter den fjärde eller femte decimalen.</span><span class="sxs-lookup"><span data-stu-id="97c28-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="97c28-116">Ta reda på om din mätare använder nivåindelade priser</span><span class="sxs-lookup"><span data-stu-id="97c28-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="97c28-117">Om du inte vet om mätaren använder nivåindelad prissättning kan du använda proceduren nedan för att ta reda på det.</span><span class="sxs-lookup"><span data-stu-id="97c28-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="97c28-118">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="97c28-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="97c28-119">Välj **Sälj,** välj **Priser och erbjudanden** och välj sedan Priser för **Azure-plan.**</span><span class="sxs-lookup"><span data-stu-id="97c28-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="97c28-120">Leta upp din mätare efter ID och ladda sedan ned dina prisdata.</span><span class="sxs-lookup"><span data-stu-id="97c28-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="97c28-121">Exempelberäkning</span><span class="sxs-lookup"><span data-stu-id="97c28-121">Sample calculation</span></span>

<span data-ttu-id="97c28-122">Tabellen nedan ger ett exempel på hur vi beräknar det effektiva enhetspriset under den öppna perioden.</span><span class="sxs-lookup"><span data-stu-id="97c28-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="97c28-123">I tabellen gäller följande värden:</span><span class="sxs-lookup"><span data-stu-id="97c28-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="97c28-124">**UP** = Enhetspris för resursen/timmen = 0,868</span><span class="sxs-lookup"><span data-stu-id="97c28-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="97c28-125">**BCU** = Fakturerbar förbrukningsenhet för mätaren</span><span class="sxs-lookup"><span data-stu-id="97c28-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="97c28-126">**BC** = Fakturerbar kostnad för mätaren = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="97c28-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="97c28-127">Detta återspeglar en justering för 15 % PEC-rabatten.</span><span class="sxs-lookup"><span data-stu-id="97c28-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="97c28-128">Sedan använder vi den nedre gränsen för funktionen för att begränsa värdet till två siffror efter decimaltecknet för att debitera det minsta beloppet.</span><span class="sxs-lookup"><span data-stu-id="97c28-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="97c28-129">**Gällande enhetspris** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="97c28-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="97c28-130">Obs! Mätaren i det här exemplet har inga prisnivåer eller andra rabatter – de effektiva enhetsprisfaktorerna i rabattprocent och andra justeringar.</span><span class="sxs-lookup"><span data-stu-id="97c28-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="97c28-131">Datum</span><span class="sxs-lookup"><span data-stu-id="97c28-131">Date</span></span> | <span data-ttu-id="97c28-132">BCU (fakturerbar förbrukningsenhet)</span><span class="sxs-lookup"><span data-stu-id="97c28-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="97c28-133">BC (fakturerbar kostnad)</span><span class="sxs-lookup"><span data-stu-id="97c28-133">BC (Billable cost)</span></span> | <span data-ttu-id="97c28-134">Effektivt enhetspris</span><span class="sxs-lookup"><span data-stu-id="97c28-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="97c28-135">3 augusti</span><span class="sxs-lookup"><span data-stu-id="97c28-135">3-Aug</span></span> | <span data-ttu-id="97c28-136">29</span><span class="sxs-lookup"><span data-stu-id="97c28-136">29</span></span> | <span data-ttu-id="97c28-137">21.39</span><span class="sxs-lookup"><span data-stu-id="97c28-137">21.39</span></span> | <span data-ttu-id="97c28-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="97c28-138">0.737586206896552</span></span> |
| <span data-ttu-id="97c28-139">10 augusti</span><span class="sxs-lookup"><span data-stu-id="97c28-139">10-Aug</span></span> | <span data-ttu-id="97c28-140">210.950039</span><span class="sxs-lookup"><span data-stu-id="97c28-140">210.950039</span></span> | <span data-ttu-id="97c28-141">155.63</span><span class="sxs-lookup"><span data-stu-id="97c28-141">155.63</span></span> | <span data-ttu-id="97c28-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="97c28-142">0.737757626107858</span></span> |
| <span data-ttu-id="97c28-143">25 augusti</span><span class="sxs-lookup"><span data-stu-id="97c28-143">25-Aug</span></span> | <span data-ttu-id="97c28-144">555.950039</span><span class="sxs-lookup"><span data-stu-id="97c28-144">555.950039</span></span> | <span data-ttu-id="97c28-145">410.17</span><span class="sxs-lookup"><span data-stu-id="97c28-145">410.17</span></span> | <span data-ttu-id="97c28-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="97c28-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="97c28-147">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="97c28-147">Next steps</span></span>

- [<span data-ttu-id="97c28-148">Fakturering och skatter</span><span class="sxs-lookup"><span data-stu-id="97c28-148">Billing and taxes</span></span>](billing.md)
