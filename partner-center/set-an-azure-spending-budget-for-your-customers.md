---
title: Ange en Azure-utgiftsbudget för kunder
ms.topic: how-to
ms.date: 03/17/2021
description: Lär dig hur du ställer in eller tar bort månatliga Azure-utgiftsbudgetar för dina kunder och hur du visar azure-utgiftsdata och anger budgetrelaterade meddelanden.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855360"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="b71a1-103">Ange, kontrollera eller ta bort månatliga Azure-utgiftsbudgetar för kunder i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="b71a1-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="b71a1-104">**Lämpliga roller:** Administratörsagent</span><span class="sxs-lookup"><span data-stu-id="b71a1-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="b71a1-105">Du kan [ange en månatlig Azure-utgiftsbudget för dina kunder](#set-azure-spending-budget) i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="b71a1-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="b71a1-106">Detta hjälper dina kunder att hantera sina Azure-utgifter.</span><span class="sxs-lookup"><span data-stu-id="b71a1-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="b71a1-107">Med det här alternativet kan du jämföra dina kunders Azure-utgifter med budgeten under månaden.</span><span class="sxs-lookup"><span data-stu-id="b71a1-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="b71a1-108">Det hjälper även dina kunder att budgetera sina Azure-utgifter så att deras månadsfaktura inte blir högre än förväntat.</span><span class="sxs-lookup"><span data-stu-id="b71a1-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="b71a1-109">Den här funktionen är inte tillgänglig i sandbox- eller Test in Production-konton (TIPS).</span><span class="sxs-lookup"><span data-stu-id="b71a1-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="b71a1-110">När du [har angett en Azure-utgiftsbudget för dina kunder](#set-azure-spending-budget)kan du även granska kundanvändningen på följande sätt.</span><span class="sxs-lookup"><span data-stu-id="b71a1-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="b71a1-111">De här alternativen kan hjälpa dig att upptäcka felkonfigurerade tjänster eller ovanliga trender som kan tyda på bedrägerier.</span><span class="sxs-lookup"><span data-stu-id="b71a1-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="b71a1-112">Du kan sedan arbeta med dina kunder för att identifiera rotorsaken och hantera kostnader.</span><span class="sxs-lookup"><span data-stu-id="b71a1-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="b71a1-113">Om det behövs kan du [också ändra kundens budget till](#set-azure-spending-budget) ett högre belopp.</span><span class="sxs-lookup"><span data-stu-id="b71a1-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="b71a1-114">Kontrollera aktuella Azure-utgifter</span><span class="sxs-lookup"><span data-stu-id="b71a1-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="b71a1-115">Aktivera e-postaviseringar när en kunds utgifter närmar sig sin budgetgräns</span><span class="sxs-lookup"><span data-stu-id="b71a1-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="b71a1-116">Visa specificerade kostnader per tjänst för användningsbaserade prenumerationer</span><span class="sxs-lookup"><span data-stu-id="b71a1-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="b71a1-117">Du kan också [ta bort en Azure-utgiftsbudget](#remove-azure-spending-budget) för kunder när som helst.</span><span class="sxs-lookup"><span data-stu-id="b71a1-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="b71a1-118">Utgiftsdata i Azure</span><span class="sxs-lookup"><span data-stu-id="b71a1-118">Azure spending data</span></span>

<span data-ttu-id="b71a1-119">Azure-utgiftsdata är en *uppskattning och* de *faktiska faktureringsbeloppen kan variera*.</span><span class="sxs-lookup"><span data-stu-id="b71a1-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="b71a1-120">Datavärdet *återspeglar inte skatter,* krediter, justeringar eller andra avgifter som kan tillkomma.</span><span class="sxs-lookup"><span data-stu-id="b71a1-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="b71a1-121">Utgiftsdata uppdateras *en gång per dag.*</span><span class="sxs-lookup"><span data-stu-id="b71a1-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="b71a1-122">Dina kunder kan fortsätta att använda (och debiteras för) Azure-tjänster och -resurser, såvida du inte ändrar deras kontoinställningar i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="b71a1-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="b71a1-123">Ange utgiftsbudget för Azure</span><span class="sxs-lookup"><span data-stu-id="b71a1-123">Set Azure spending budget</span></span>

<span data-ttu-id="b71a1-124">Du kan *ange en månatlig Azure-utgiftsbudget* för flera kunder i Partnercenter:</span><span class="sxs-lookup"><span data-stu-id="b71a1-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="b71a1-125">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="b71a1-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="b71a1-126">I den vänstra menyn under **CSP väljer** du **Azure-utgifter.**</span><span class="sxs-lookup"><span data-stu-id="b71a1-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="b71a1-127">På **sidan Azure-utgifter** under **Kunder med Microsoft Azure prenumerationer** väljer du de kunder som du vill ange en budget för.</span><span class="sxs-lookup"><span data-stu-id="b71a1-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="b71a1-128">Ange ett värde för **Månadsbudget**.</span><span class="sxs-lookup"><span data-stu-id="b71a1-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="b71a1-129">Välj **Tillämpa** för att spara ändringarna.</span><span class="sxs-lookup"><span data-stu-id="b71a1-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="b71a1-130">Du kan också *ange en budget för en enskild kund* i prenumerationsinställningarna:</span><span class="sxs-lookup"><span data-stu-id="b71a1-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="b71a1-131">Logga in på instrumentpanelen i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="b71a1-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="b71a1-132">I den vänstra menyn under **CSP väljer** du **Kunder.**</span><span class="sxs-lookup"><span data-stu-id="b71a1-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="b71a1-133">På **sidan** Kunder väljer du kundens **företagsnamn**.</span><span class="sxs-lookup"><span data-stu-id="b71a1-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="b71a1-134">På kundens sida **Prenumerationer, under** **Användningsbaserad prenumeration,** väljer du **Ändra budget.**</span><span class="sxs-lookup"><span data-stu-id="b71a1-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="b71a1-135">Ange ett värde för budgeten.</span><span class="sxs-lookup"><span data-stu-id="b71a1-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="b71a1-136">Välj **Tillämpa** för att spara ändringarna.</span><span class="sxs-lookup"><span data-stu-id="b71a1-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="b71a1-137">Ta bort utgiftsbudgeten i Azure</span><span class="sxs-lookup"><span data-stu-id="b71a1-137">Remove Azure spending budget</span></span>

<span data-ttu-id="b71a1-138">Du kan *ta bort en månatlig Azure-utgiftsbudget* för dina kunder i Partnercenter:</span><span class="sxs-lookup"><span data-stu-id="b71a1-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="b71a1-139">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="b71a1-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="b71a1-140">I den vänstra menyn under **CSP väljer** du **Azure-utgifter.**</span><span class="sxs-lookup"><span data-stu-id="b71a1-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="b71a1-141">På sidan **Azure-utgifter** under **Kunder med Microsoft Azure prenumerationer** väljer du de kunder vars budget du vill ta bort.</span><span class="sxs-lookup"><span data-stu-id="b71a1-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="b71a1-142">Välj **Ta bort budget.**</span><span class="sxs-lookup"><span data-stu-id="b71a1-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="b71a1-143">Kontrollera aktuella Azure-utgifter</span><span class="sxs-lookup"><span data-stu-id="b71a1-143">Check current Azure spending</span></span>

<span data-ttu-id="b71a1-144">Du kan *spåra dina kunders aktuella Azure-utgifter och månadsbudgetar* när som helst:</span><span class="sxs-lookup"><span data-stu-id="b71a1-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="b71a1-145">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="b71a1-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="b71a1-146">På den vänstra menyn under **CSP väljer** du **Azure-utgifter.**</span><span class="sxs-lookup"><span data-stu-id="b71a1-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="b71a1-147">På **sidan Azure-utgifter** under **Kunder med Microsoft Azure prenumerationer** kan du se en översikt över kundernas månatliga budgetar, aktuella utgiftsuppskattningar och procentandelen budget som används.</span><span class="sxs-lookup"><span data-stu-id="b71a1-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="b71a1-148">Meddelanden om budgetgränser</span><span class="sxs-lookup"><span data-stu-id="b71a1-148">Notifications for budget limits</span></span>

<span data-ttu-id="b71a1-149">Du kan *aktivera e-postaviseringar* när kundens månatliga utgifter närmar sig sin budgetgräns.</span><span class="sxs-lookup"><span data-stu-id="b71a1-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="b71a1-150">När du aktiverar det här alternativet får du ett meddelande när kunderna använder 80 % eller mer av sin månadsbudget.</span><span class="sxs-lookup"><span data-stu-id="b71a1-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="b71a1-151">Det här alternativet hjälper dig att hålla ett öga på Din Azure-faktura.</span><span class="sxs-lookup"><span data-stu-id="b71a1-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="b71a1-152">Så här konfigurerar du e-postaviseringar:</span><span class="sxs-lookup"><span data-stu-id="b71a1-152">To configure email notifications:</span></span>

1. <span data-ttu-id="b71a1-153">Logga in på Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b71a1-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="b71a1-154">Gå till **Inställningar**.</span><span class="sxs-lookup"><span data-stu-id="b71a1-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="b71a1-155">Välj **Mina inställningar.**</span><span class="sxs-lookup"><span data-stu-id="b71a1-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="b71a1-156">Konfigurera en önskad e-postadress om du inte har gjort det.</span><span class="sxs-lookup"><span data-stu-id="b71a1-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="b71a1-157">Konfigurera önskat språk för meddelandet.</span><span class="sxs-lookup"><span data-stu-id="b71a1-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="b71a1-158">Välj **fliken CSP** under **avsnittet Meddelandeinställningar.**</span><span class="sxs-lookup"><span data-stu-id="b71a1-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="b71a1-159">Markera alternativet E-post för Azure Spending notification **(Azure-utgiftsavisering)** och **Spara**.</span><span class="sxs-lookup"><span data-stu-id="b71a1-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="b71a1-160">Specificerade kostnader per tjänst</span><span class="sxs-lookup"><span data-stu-id="b71a1-160">Itemized costs by service</span></span>

<span data-ttu-id="b71a1-161">Du kan *visa specificerade kostnader (och beräknad användning) per tjänst för användningsbaserade prenumerationer:*</span><span class="sxs-lookup"><span data-stu-id="b71a1-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="b71a1-162">Logga in på Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b71a1-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="b71a1-163">I den vänstra menyn under **CSP väljer** du **Kunder.**</span><span class="sxs-lookup"><span data-stu-id="b71a1-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="b71a1-164">På **sidan** Kunder väljer du kundens **företagsnamn**.</span><span class="sxs-lookup"><span data-stu-id="b71a1-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="b71a1-165">På kundens **prenumerationssida** går du till **Användningsbaserade prenumerationer** och väljer namnet på **Prenumeration.**</span><span class="sxs-lookup"><span data-stu-id="b71a1-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="b71a1-166">På prenumerationens sida kan du granska De beräknade **kostnaderna** per tjänst och **Beräknad användning för** den aktuella månaden.</span><span class="sxs-lookup"><span data-stu-id="b71a1-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="b71a1-167">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="b71a1-167">Next steps</span></span>

- [<span data-ttu-id="b71a1-168">Ny handelsupplevelse i CSP – Azure-fakturering</span><span class="sxs-lookup"><span data-stu-id="b71a1-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
