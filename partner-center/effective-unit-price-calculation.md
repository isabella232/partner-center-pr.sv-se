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
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147130"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="759fb-104">Effektiv enhetsprisberäkning för Förbrukning i Azure-plan</span><span class="sxs-lookup"><span data-stu-id="759fb-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="759fb-105">**Lämpliga roller:** Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="759fb-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="759fb-106">Det effektiva enhetspriset</span><span class="sxs-lookup"><span data-stu-id="759fb-106">The effective unit price</span></span>

<span data-ttu-id="759fb-107">Det effektiva enhetspriset beräknas på mätarnivå (till skillnad från resursnivån) och justeras dagligen enligt mätaranvändningen.</span><span class="sxs-lookup"><span data-stu-id="759fb-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="759fb-108">Vi beräknar det effektiva enhetspriset med hjälp av följande tre faktorer:</span><span class="sxs-lookup"><span data-stu-id="759fb-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="759fb-109">Förbrukning, som övervakas dagligen under faktureringsperioden</span><span class="sxs-lookup"><span data-stu-id="759fb-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="759fb-110">Fakturerbar kostnad för mätaren</span><span class="sxs-lookup"><span data-stu-id="759fb-110">Billable cost for the meter</span></span>
- <span data-ttu-id="759fb-111">Nivåindelad (om tillämpligt)</span><span class="sxs-lookup"><span data-stu-id="759fb-111">Tiering (if applicable)</span></span>

<span data-ttu-id="759fb-112">Eftersom vi övervakar förbrukningen varje dag under faktureringsperioden varierar det effektiva enhetspriset.</span><span class="sxs-lookup"><span data-stu-id="759fb-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="759fb-113">Det slutliga priset för en viss faktureringsperiod blir tillgängligt när vi stoppar förbrukningsberäkningen och stänger faktureringsperioden.</span><span class="sxs-lookup"><span data-stu-id="759fb-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="759fb-114">Du ser de flesta förbrukningsändringarna efter den fjärde eller femte decimalen.</span><span class="sxs-lookup"><span data-stu-id="759fb-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="759fb-115">Ta reda på om din mätare använder nivåindelade priser</span><span class="sxs-lookup"><span data-stu-id="759fb-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="759fb-116">Om du inte vet om mätaren använder nivåindelad prissättning kan du använda proceduren nedan för att ta reda på det.</span><span class="sxs-lookup"><span data-stu-id="759fb-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="759fb-117">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="759fb-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="759fb-118">Välj **Sälj,** välj **Priser och erbjudanden** och välj sedan Priser för **Azure-plan.**</span><span class="sxs-lookup"><span data-stu-id="759fb-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="759fb-119">Leta upp din mätare efter ID och ladda sedan ned dina prisdata.</span><span class="sxs-lookup"><span data-stu-id="759fb-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="759fb-120">Exempelberäkning</span><span class="sxs-lookup"><span data-stu-id="759fb-120">Sample calculation</span></span>

<span data-ttu-id="759fb-121">Tabellen nedan ger ett exempel på hur vi beräknar det effektiva enhetspriset under den öppna perioden.</span><span class="sxs-lookup"><span data-stu-id="759fb-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="759fb-122">I tabellen gäller följande värden:</span><span class="sxs-lookup"><span data-stu-id="759fb-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="759fb-123">**UP** = Enhetspris för resursen/timmen = 0,868</span><span class="sxs-lookup"><span data-stu-id="759fb-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="759fb-124">**BCU** = Fakturerbar förbrukningsenhet för mätaren</span><span class="sxs-lookup"><span data-stu-id="759fb-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="759fb-125">**BC** = Fakturerbar kostnad för mätaren = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="759fb-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="759fb-126">Detta återspeglar en justering för 15 % PEC-rabatten.</span><span class="sxs-lookup"><span data-stu-id="759fb-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="759fb-127">Sedan använder vi den nedre gränsen för funktionen för att begränsa värdet till två siffror efter decimaltecknet för att debitera det minsta beloppet.</span><span class="sxs-lookup"><span data-stu-id="759fb-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="759fb-128">**Effektivt enhetspris** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="759fb-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="759fb-129">Obs! Mätaren i det här exemplet har inga prisnivåer eller andra rabatter – de effektiva enhetsprisfaktorerna i rabattprocent och andra justeringar.</span><span class="sxs-lookup"><span data-stu-id="759fb-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="759fb-130">Datum</span><span class="sxs-lookup"><span data-stu-id="759fb-130">Date</span></span> | <span data-ttu-id="759fb-131">BCU (fakturerbar förbrukningsenhet)</span><span class="sxs-lookup"><span data-stu-id="759fb-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="759fb-132">BC (fakturerbar kostnad)</span><span class="sxs-lookup"><span data-stu-id="759fb-132">BC (Billable cost)</span></span> | <span data-ttu-id="759fb-133">Effektivt enhetspris</span><span class="sxs-lookup"><span data-stu-id="759fb-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="759fb-134">3 augusti</span><span class="sxs-lookup"><span data-stu-id="759fb-134">3-Aug</span></span> | <span data-ttu-id="759fb-135">29</span><span class="sxs-lookup"><span data-stu-id="759fb-135">29</span></span> | <span data-ttu-id="759fb-136">21.39</span><span class="sxs-lookup"><span data-stu-id="759fb-136">21.39</span></span> | <span data-ttu-id="759fb-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="759fb-137">0.737586206896552</span></span> |
| <span data-ttu-id="759fb-138">10 augusti</span><span class="sxs-lookup"><span data-stu-id="759fb-138">10-Aug</span></span> | <span data-ttu-id="759fb-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="759fb-139">210.950039</span></span> | <span data-ttu-id="759fb-140">155.63</span><span class="sxs-lookup"><span data-stu-id="759fb-140">155.63</span></span> | <span data-ttu-id="759fb-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="759fb-141">0.737757626107858</span></span> |
| <span data-ttu-id="759fb-142">25 augusti</span><span class="sxs-lookup"><span data-stu-id="759fb-142">25-Aug</span></span> | <span data-ttu-id="759fb-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="759fb-143">555.950039</span></span> | <span data-ttu-id="759fb-144">410.17</span><span class="sxs-lookup"><span data-stu-id="759fb-144">410.17</span></span> | <span data-ttu-id="759fb-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="759fb-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="759fb-146">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="759fb-146">Next steps</span></span>

- [<span data-ttu-id="759fb-147">Fakturering och skatter</span><span class="sxs-lookup"><span data-stu-id="759fb-147">Billing and taxes</span></span>](billing.md)
