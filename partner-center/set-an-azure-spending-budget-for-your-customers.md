---
title: Ange en Azure utgifts budget för kunder
ms.topic: how-to
ms.date: 06/03/2020
description: Lär dig hur du ställer in eller tar bort månads utgifter för Azure-utgifter för dina kunder och även för att Visa Azures utgifts data och ange budgetrelaterade aviseringar.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 982d4ed310415349acde3d260afce04eb0d55ac5
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2020
ms.locfileid: "92531213"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="b9b3d-103">Ange, kontrol lera eller ta bort månads utgifts budgetar för kunder i Partner Center</span><span class="sxs-lookup"><span data-stu-id="b9b3d-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="b9b3d-104">Gäller för:</span><span class="sxs-lookup"><span data-stu-id="b9b3d-104">Applies to:</span></span>

- <span data-ttu-id="b9b3d-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="b9b3d-105">Partner Center</span></span>
- <span data-ttu-id="b9b3d-106">Partner Center för Microsoft Cloud för amerikanska myndigheter</span><span class="sxs-lookup"><span data-stu-id="b9b3d-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="b9b3d-107">Du kan [ställa in en månatlig Azure utgifts budget för dina kunder](#set-azure-spending-budget) i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="b9b3d-108">Detta hjälper kunderna att hantera sina Azure-utgifter.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="b9b3d-109">Med det här alternativet kan du jämföra kundernas Azure-utgifter i budgeten under månaden.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="b9b3d-110">Det hjälper också kunderna att budgetera sina Azure-utgifter så att deras månatliga faktura inte är högre än förväntat.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="b9b3d-111">Den här funktionen är inte tillgänglig i ett begränsat läge eller test i produktions konton (TIP).</span><span class="sxs-lookup"><span data-stu-id="b9b3d-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="b9b3d-112">När du [har ställt in en Azure utgifts budget för din kund (er)](#set-azure-spending-budget)kan du också granska kund användningen på följande sätt.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="b9b3d-113">De här alternativen kan hjälpa dig att hitta felkonfigurerade tjänster eller ovanliga trender som kan föreslå bedrägerier.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="b9b3d-114">Sedan kan du arbeta med din kund (er) för att identifiera rotor saken och hantera kostnader.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="b9b3d-115">Om det behövs kan du även [ändra kundens budget](#set-azure-spending-budget) till en högre mängd.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="b9b3d-116">Kontrol lera aktuella Azure-utgifter</span><span class="sxs-lookup"><span data-stu-id="b9b3d-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="b9b3d-117">Aktivera e-postaviseringar för när en kunds utgifter närmar sig sin budget gräns</span><span class="sxs-lookup"><span data-stu-id="b9b3d-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="b9b3d-118">Visa specificerade kostnader per tjänst för användnings prenumerationer</span><span class="sxs-lookup"><span data-stu-id="b9b3d-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="b9b3d-119">Du kan också [ta bort en Azure utgifts budget](#remove-azure-spending-budget) för kunder när som helst.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="b9b3d-120">Azure-utgifts data</span><span class="sxs-lookup"><span data-stu-id="b9b3d-120">Azure spending data</span></span>

<span data-ttu-id="b9b3d-121">Azures utgifts data är en *uppskattning* och de *faktiska fakturerings beloppen kan variera* .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-121">The Azure spending data is an *estimate* and *actual billing amounts may vary* .</span></span> <span data-ttu-id="b9b3d-122">Data svärdet *återspeglar inte* skatter, krediter, justeringar eller andra avgifter som kan tillkomma.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="b9b3d-123">Utgifts informationen *uppdateras en gång per dag* .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-123">The spending data is *refreshed once per day* .</span></span> <span data-ttu-id="b9b3d-124">Dina kunder kan fortsätta att använda (och debiteras för) Azure-tjänster och-resurser, om du inte ändrar konto inställningarna i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="b9b3d-125">Ställ in Azure utgifts budget</span><span class="sxs-lookup"><span data-stu-id="b9b3d-125">Set Azure spending budget</span></span>

<span data-ttu-id="b9b3d-126">Du kan *ställa in en månatlig Azure utgifts budget* för flera kunder i Partner Center:</span><span class="sxs-lookup"><span data-stu-id="b9b3d-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="b9b3d-127">Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="b9b3d-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="b9b3d-128">Välj **Azure-utgifter** i den vänstra menyn under **CSP** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-128">In the left-hand menu under **CSP** , choose **Azure spending** .</span></span>

3. <span data-ttu-id="b9b3d-129">På sidan **Azure-utgifter** under **kunder med Microsoft Azure prenumerationer** väljer du de kunder för vilka du vill ställa in en budget.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions** , select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="b9b3d-130">Ange ett värde för **månatlig budget** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-130">Enter a value for **Monthly budget** .</span></span>

5. <span data-ttu-id="b9b3d-131">Välj **Verkställ** för att spara ändringarna.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="b9b3d-132">Du kan också *Ange en budget för en enskild kund* i prenumerations inställningarna:</span><span class="sxs-lookup"><span data-stu-id="b9b3d-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="b9b3d-133">Logga in på Partner Center-instrumentpanelen.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="b9b3d-134">Välj **kunder** i den vänstra menyn under **CSP** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-134">In the left-hand menu under **CSP** , choose **Customers** .</span></span>

3. <span data-ttu-id="b9b3d-135">På sidan **kunder** väljer du kundens **företags namn** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-135">On the **Customers** page, select the customer's **Company name** .</span></span>

4. <span data-ttu-id="b9b3d-136">På sidan kund **prenumerationer** , under **användnings-baserad prenumeration** , väljer du **ändra budget** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-136">On the customer's **Subscriptions** page, under **Usage-based subscription** , choose **Change budget** .</span></span>

5. <span data-ttu-id="b9b3d-137">Ange ett värde för budgeten.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="b9b3d-138">Välj **Verkställ** för att spara ändringarna.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="b9b3d-139">Ta bort utgifts budget för Azure</span><span class="sxs-lookup"><span data-stu-id="b9b3d-139">Remove Azure spending budget</span></span>

<span data-ttu-id="b9b3d-140">Du kan *ta bort en månatlig Azure utgifts budget* för din kund (er) i Partner Center:</span><span class="sxs-lookup"><span data-stu-id="b9b3d-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="b9b3d-141">Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="b9b3d-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="b9b3d-142">Välj **Azure-utgifter** i den vänstra menyn under **CSP** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-142">In the left-hand menu under **CSP** , choose **Azure spending** .</span></span>

3. <span data-ttu-id="b9b3d-143">På sidan **Azure-utgifter** under **kunder med Microsoft Azure prenumerationer** väljer du den eller de kunder vars budget du vill ta bort.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions** , select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="b9b3d-144">Välj **ta bort budget** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-144">Choose **Remove budget** .</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="b9b3d-145">Kontrol lera aktuella Azure-utgifter</span><span class="sxs-lookup"><span data-stu-id="b9b3d-145">Check current Azure spending</span></span>

<span data-ttu-id="b9b3d-146">Du kan när som helst *spåra kundernas aktuella Azure-utgifter och månads budgetar* :</span><span class="sxs-lookup"><span data-stu-id="b9b3d-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="b9b3d-147">Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="b9b3d-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="b9b3d-148">Välj **Azure-utgifter** i den vänstra menyn under **CSP** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-148">In the left-hand menu under **CSP** , choose **Azure spending** .</span></span>

3. <span data-ttu-id="b9b3d-149">På sidan **Azure-utgifter** under **kunder med Microsoft Azure prenumerationer** kan du se en översikt över kunders månads budgetar, aktuella utgifts uppskattningar och procent andel av budgeten som används.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions** , you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="b9b3d-150">Meddelanden för budget gränser</span><span class="sxs-lookup"><span data-stu-id="b9b3d-150">Notifications for budget limits</span></span>

<span data-ttu-id="b9b3d-151">Du kan *Aktivera e-postaviseringar* för när kundens månads utgifter närmar sig budget gränsen.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="b9b3d-152">När du aktiverar det här alternativet får du ett meddelande när kunderna använder 80% eller mer av sin månads budget.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="b9b3d-153">Det här alternativet hjälper dig att hålla ett öga på din Azure-faktura.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="b9b3d-154">Så här konfigurerar du e-postmeddelanden:</span><span class="sxs-lookup"><span data-stu-id="b9b3d-154">To configure email notifications:</span></span>

1. <span data-ttu-id="b9b3d-155">Logga in på Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="b9b3d-156">Välj **Azure-utgifter** i den vänstra menyn under **CSP** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-156">In the left-hand menu under **CSP** , choose **Azure spending** .</span></span>

3. <span data-ttu-id="b9b3d-157">På sidan **Azure-utgifter** , under **e-postaviseringar** , kan du växla inställningen **Hämta e-post** till **på** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-157">On the **Azure spending** page, under **Email notifications** , toggle the **Get emails** setting to **On** .</span></span>

4. <span data-ttu-id="b9b3d-158">Välj **ändra e-postadress** för att se e-postadressen för meddelanden.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-158">Choose **Change email address** to see the email address for notifications.</span></span>

5. <span data-ttu-id="b9b3d-159">Om e-postadressen *inte är korrekt* anger du rätt e-postadress och väljer **Uppdatera** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-159">If the email address *isn't correct* , enter the correct email address and choose **Update** .</span></span> <span data-ttu-id="b9b3d-160">Om e-postadressen *är korrekt* väljer du **Avbryt** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-160">If the email address *is correct* , choose **Cancel** .</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="b9b3d-161">Specificerade kostnader per tjänst</span><span class="sxs-lookup"><span data-stu-id="b9b3d-161">Itemized costs by service</span></span>

<span data-ttu-id="b9b3d-162">Du kan *Visa de specificerade kostnaderna (och den uppskattade användningen) efter tjänst för användnings-baserade prenumerationer* :</span><span class="sxs-lookup"><span data-stu-id="b9b3d-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions* :</span></span>

1. <span data-ttu-id="b9b3d-163">Logga in på Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="b9b3d-164">Välj **kunder** i den vänstra menyn under **CSP** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-164">In the left-hand menu under **CSP** , choose **Customers** .</span></span>

3. <span data-ttu-id="b9b3d-165">På sidan **kunder** väljer du kundens **företags namn** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-165">On the **Customers** page, select the customer's **Company name** .</span></span>

4. <span data-ttu-id="b9b3d-166">På sidan kund **prenumerationer** under **användnings prenumerationer** väljer du namnet på **prenumerationen** .</span><span class="sxs-lookup"><span data-stu-id="b9b3d-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions** , select the name of the **Subscription** .</span></span>

5. <span data-ttu-id="b9b3d-167">På prenumerationens sida kan du granska de **specificerade kostnaderna** per tjänst och den **beräknade användningen** för den aktuella månaden.</span><span class="sxs-lookup"><span data-stu-id="b9b3d-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
