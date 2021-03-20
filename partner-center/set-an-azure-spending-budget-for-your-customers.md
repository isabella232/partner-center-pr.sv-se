---
title: Ange en Azure-utgiftsbudget för kunder
ms.topic: how-to
ms.date: 03/17/2021
description: Lär dig hur du ställer in eller tar bort månads utgifter för Azure-utgifter för dina kunder och även för att Visa Azures utgifts data och ange budgetrelaterade aviseringar.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712757"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="84cee-103">Ange, kontrol lera eller ta bort månads utgifts budgetar för kunder i Partner Center</span><span class="sxs-lookup"><span data-stu-id="84cee-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="84cee-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="84cee-104">**Appropriate roles**</span></span>

- <span data-ttu-id="84cee-105">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="84cee-105">Admin agent</span></span>

<span data-ttu-id="84cee-106">Du kan [ställa in en månatlig Azure utgifts budget för dina kunder](#set-azure-spending-budget) i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="84cee-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="84cee-107">Detta hjälper kunderna att hantera sina Azure-utgifter.</span><span class="sxs-lookup"><span data-stu-id="84cee-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="84cee-108">Med det här alternativet kan du jämföra kundernas Azure-utgifter i budgeten under månaden.</span><span class="sxs-lookup"><span data-stu-id="84cee-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="84cee-109">Det hjälper också kunderna att budgetera sina Azure-utgifter så att deras månatliga faktura inte är högre än förväntat.</span><span class="sxs-lookup"><span data-stu-id="84cee-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="84cee-110">Den här funktionen är inte tillgänglig i ett begränsat läge eller test i produktions konton (TIP).</span><span class="sxs-lookup"><span data-stu-id="84cee-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="84cee-111">När du [har ställt in en Azure utgifts budget för din kund (er)](#set-azure-spending-budget)kan du också granska kund användningen på följande sätt.</span><span class="sxs-lookup"><span data-stu-id="84cee-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="84cee-112">De här alternativen kan hjälpa dig att hitta felkonfigurerade tjänster eller ovanliga trender som kan föreslå bedrägerier.</span><span class="sxs-lookup"><span data-stu-id="84cee-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="84cee-113">Sedan kan du arbeta med din kund (er) för att identifiera rotor saken och hantera kostnader.</span><span class="sxs-lookup"><span data-stu-id="84cee-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="84cee-114">Om det behövs kan du även [ändra kundens budget](#set-azure-spending-budget) till en högre mängd.</span><span class="sxs-lookup"><span data-stu-id="84cee-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="84cee-115">Kontrol lera aktuella Azure-utgifter</span><span class="sxs-lookup"><span data-stu-id="84cee-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="84cee-116">Aktivera e-postaviseringar för när en kunds utgifter närmar sig sin budget gräns</span><span class="sxs-lookup"><span data-stu-id="84cee-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="84cee-117">Visa specificerade kostnader per tjänst för användnings prenumerationer</span><span class="sxs-lookup"><span data-stu-id="84cee-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="84cee-118">Du kan också [ta bort en Azure utgifts budget](#remove-azure-spending-budget) för kunder när som helst.</span><span class="sxs-lookup"><span data-stu-id="84cee-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="84cee-119">Azure-utgifts data</span><span class="sxs-lookup"><span data-stu-id="84cee-119">Azure spending data</span></span>

<span data-ttu-id="84cee-120">Azures utgifts data är en *uppskattning* och de *faktiska fakturerings beloppen kan variera*.</span><span class="sxs-lookup"><span data-stu-id="84cee-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="84cee-121">Data svärdet *återspeglar inte* skatter, krediter, justeringar eller andra avgifter som kan tillkomma.</span><span class="sxs-lookup"><span data-stu-id="84cee-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="84cee-122">Utgifts informationen *uppdateras en gång per dag*.</span><span class="sxs-lookup"><span data-stu-id="84cee-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="84cee-123">Dina kunder kan fortsätta att använda (och debiteras för) Azure-tjänster och-resurser, om du inte ändrar konto inställningarna i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="84cee-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="84cee-124">Ställ in Azure utgifts budget</span><span class="sxs-lookup"><span data-stu-id="84cee-124">Set Azure spending budget</span></span>

<span data-ttu-id="84cee-125">Du kan *ställa in en månatlig Azure utgifts budget* för flera kunder i Partner Center:</span><span class="sxs-lookup"><span data-stu-id="84cee-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="84cee-126">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="84cee-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="84cee-127">Välj **Azure-utgifter** i den vänstra menyn under **CSP**.</span><span class="sxs-lookup"><span data-stu-id="84cee-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="84cee-128">På sidan **Azure-utgifter** under **kunder med Microsoft Azure prenumerationer** väljer du de kunder för vilka du vill ställa in en budget.</span><span class="sxs-lookup"><span data-stu-id="84cee-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="84cee-129">Ange ett värde för **månatlig budget**.</span><span class="sxs-lookup"><span data-stu-id="84cee-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="84cee-130">Välj **Verkställ** för att spara ändringarna.</span><span class="sxs-lookup"><span data-stu-id="84cee-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="84cee-131">Du kan också *Ange en budget för en enskild kund* i prenumerations inställningarna:</span><span class="sxs-lookup"><span data-stu-id="84cee-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="84cee-132">Logga in på instrumentpanelen i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="84cee-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="84cee-133">Välj **kunder** i den vänstra menyn under **CSP**.</span><span class="sxs-lookup"><span data-stu-id="84cee-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="84cee-134">På sidan **kunder** väljer du kundens **företags namn**.</span><span class="sxs-lookup"><span data-stu-id="84cee-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="84cee-135">På sidan kund **prenumerationer** , under **användnings-baserad prenumeration**, väljer du **ändra budget**.</span><span class="sxs-lookup"><span data-stu-id="84cee-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="84cee-136">Ange ett värde för budgeten.</span><span class="sxs-lookup"><span data-stu-id="84cee-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="84cee-137">Välj **Verkställ** för att spara ändringarna.</span><span class="sxs-lookup"><span data-stu-id="84cee-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="84cee-138">Ta bort utgifts budget för Azure</span><span class="sxs-lookup"><span data-stu-id="84cee-138">Remove Azure spending budget</span></span>

<span data-ttu-id="84cee-139">Du kan *ta bort en månatlig Azure utgifts budget* för din kund (er) i Partner Center:</span><span class="sxs-lookup"><span data-stu-id="84cee-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="84cee-140">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="84cee-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="84cee-141">Välj **Azure-utgifter** i den vänstra menyn under **CSP**.</span><span class="sxs-lookup"><span data-stu-id="84cee-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="84cee-142">På sidan **Azure-utgifter** under **kunder med Microsoft Azure prenumerationer** väljer du den eller de kunder vars budget du vill ta bort.</span><span class="sxs-lookup"><span data-stu-id="84cee-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="84cee-143">Välj **ta bort budget**.</span><span class="sxs-lookup"><span data-stu-id="84cee-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="84cee-144">Kontrol lera aktuella Azure-utgifter</span><span class="sxs-lookup"><span data-stu-id="84cee-144">Check current Azure spending</span></span>

<span data-ttu-id="84cee-145">Du kan när som helst *spåra kundernas aktuella Azure-utgifter och månads budgetar* :</span><span class="sxs-lookup"><span data-stu-id="84cee-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="84cee-146">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="84cee-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="84cee-147">Välj **Azure-utgifter** i den vänstra menyn under **CSP**.</span><span class="sxs-lookup"><span data-stu-id="84cee-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="84cee-148">På sidan **Azure-utgifter** under **kunder med Microsoft Azure prenumerationer** kan du se en översikt över kunders månads budgetar, aktuella utgifts uppskattningar och procent andel av budgeten som används.</span><span class="sxs-lookup"><span data-stu-id="84cee-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="84cee-149">Meddelanden för budget gränser</span><span class="sxs-lookup"><span data-stu-id="84cee-149">Notifications for budget limits</span></span>

<span data-ttu-id="84cee-150">Du kan *Aktivera e-postaviseringar* för när kundens månads utgifter närmar sig budget gränsen.</span><span class="sxs-lookup"><span data-stu-id="84cee-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="84cee-151">När du aktiverar det här alternativet får du ett meddelande när kunderna använder 80% eller mer av sin månads budget.</span><span class="sxs-lookup"><span data-stu-id="84cee-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="84cee-152">Det här alternativet hjälper dig att hålla ett öga på din Azure-faktura.</span><span class="sxs-lookup"><span data-stu-id="84cee-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="84cee-153">Så här konfigurerar du e-postmeddelanden:</span><span class="sxs-lookup"><span data-stu-id="84cee-153">To configure email notifications:</span></span>

1. <span data-ttu-id="84cee-154">Logga in på Partner Center.</span><span class="sxs-lookup"><span data-stu-id="84cee-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="84cee-155">Gå till **Inställningar**.</span><span class="sxs-lookup"><span data-stu-id="84cee-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="84cee-156">Välj **Mina inställningar**.</span><span class="sxs-lookup"><span data-stu-id="84cee-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="84cee-157">Konfigurera en önskad e-postadress om du inte har det.</span><span class="sxs-lookup"><span data-stu-id="84cee-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="84cee-158">Konfigurera det prioriterade språket för meddelandet.</span><span class="sxs-lookup"><span data-stu-id="84cee-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="84cee-159">Välj fliken **kryptografiprovider** under avsnittet **aviserings inställningar** .</span><span class="sxs-lookup"><span data-stu-id="84cee-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="84cee-160">Kontrol lera e-postalternativet för **Azure utgifts** meddelande och **Spara**.</span><span class="sxs-lookup"><span data-stu-id="84cee-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="84cee-161">Specificerade kostnader per tjänst</span><span class="sxs-lookup"><span data-stu-id="84cee-161">Itemized costs by service</span></span>

<span data-ttu-id="84cee-162">Du kan *Visa de specificerade kostnaderna (och den uppskattade användningen) efter tjänst för användnings-baserade prenumerationer*:</span><span class="sxs-lookup"><span data-stu-id="84cee-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="84cee-163">Logga in på Partner Center.</span><span class="sxs-lookup"><span data-stu-id="84cee-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="84cee-164">Välj **kunder** i den vänstra menyn under **CSP**.</span><span class="sxs-lookup"><span data-stu-id="84cee-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="84cee-165">På sidan **kunder** väljer du kundens **företags namn**.</span><span class="sxs-lookup"><span data-stu-id="84cee-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="84cee-166">På sidan kund **prenumerationer** under **användnings prenumerationer** väljer du namnet på **prenumerationen**.</span><span class="sxs-lookup"><span data-stu-id="84cee-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="84cee-167">På prenumerationens sida kan du granska de **specificerade kostnaderna** per tjänst och den **beräknade användningen** för den aktuella månaden.</span><span class="sxs-lookup"><span data-stu-id="84cee-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="84cee-168">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="84cee-168">Next steps</span></span>

- [<span data-ttu-id="84cee-169">Ny handelsupplevelse i CSP – Azure-fakturering</span><span class="sxs-lookup"><span data-stu-id="84cee-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
