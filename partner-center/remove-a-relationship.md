---
title: Ta bort återförsäljarrelationen med en kund
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ta reda på hur Microsofts direktpartner kan ta bort kunder från listan, ta bort delegerade administratörsbehörigheter och sluta stödja eller köpa för en kund.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 83259f2f895be9ef34c55db5613ccfe6891a4424
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551477"
---
# <a name="how-to-remove-a-reseller-relationship-with-a-customer-in-partner-center"></a><span data-ttu-id="35824-103">Så här tar du bort en återförsäljarrelation med en kund i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="35824-103">How to remove a reseller relationship with a customer in Partner Center</span></span>

<span data-ttu-id="35824-104">**Lämpliga roller:** Global administratör</span><span class="sxs-lookup"><span data-stu-id="35824-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="35824-105">I den här artikeln beskrivs hur du tar bort en återförsäljarrelation med en kund i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="35824-105">This article describes how to remove a reseller relationship with a customer in Partner Center.</span></span>

<span data-ttu-id="35824-106">Direkta partner eller indirekta leverantörer: Om du inte längre gör en kontakt med en kund kan du ta bort relationen i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="35824-106">Direct partners or Indirect providers: if you're no longer transacting with a customer, you can remove the relationship in Partner Center.</span></span>

<span data-ttu-id="35824-107">Borttagning av en relation har följande konsekvenser:</span><span class="sxs-lookup"><span data-stu-id="35824-107">Removing a relationship has the following consequences:</span></span>

- <span data-ttu-id="35824-108">Kunden tas bort från din lista över kunder i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="35824-108">Removes the customer from your list of customers in Partner Center</span></span>
- <span data-ttu-id="35824-109">Tar bort dig från [listan över tillgängliga supportkontakter](assign-support-contacts.md) för din kund</span><span class="sxs-lookup"><span data-stu-id="35824-109">Removes you from the [list of available support contacts](assign-support-contacts.md) for your customer</span></span>
- <span data-ttu-id="35824-110">Dina administratörsprivilegier för delegering för kunden tas bort</span><span class="sxs-lookup"><span data-stu-id="35824-110">Removes your delegation admin privileges for the customer</span></span>
- <span data-ttu-id="35824-111">Du kan inte göra framtida inköp för kunden</span><span class="sxs-lookup"><span data-stu-id="35824-111">Prevents you from making future purchases for the customer</span></span>

## <a name="how-to-remove-a-relationship"></a><span data-ttu-id="35824-112">Ta bort en relation</span><span class="sxs-lookup"><span data-stu-id="35824-112">How to remove a relationship</span></span>

<span data-ttu-id="35824-113">Om du vill ta bort relationen måste du avbryta reservationer för reserverad Azure-instans (RI), avbryta programvaruinköp och inaktivera eventuella återstående aktiva prenumerationer först.</span><span class="sxs-lookup"><span data-stu-id="35824-113">To remove the relationship, you'll need to cancel Azure reserved instance (RI) reservations, cancel software purchases, and suspend any remaining active subscriptions first.</span></span>

1. <span data-ttu-id="35824-114">**Pausa alla aktiva prenumerationer.**</span><span class="sxs-lookup"><span data-stu-id="35824-114">**Suspend any active subscriptions.**</span></span>

   1. <span data-ttu-id="35824-115">Från Partnercenter går du till **Kunder** och väljer en kund</span><span class="sxs-lookup"><span data-stu-id="35824-115">From the Partner Center, go to **Customers** and select a customer</span></span>

   2. <span data-ttu-id="35824-116">Under **Prenumerationer** väljer du en prenumeration.</span><span class="sxs-lookup"><span data-stu-id="35824-116">Under **Subscriptions**, select a subscription.</span></span>

   3. <span data-ttu-id="35824-117">Välj **Pausad**</span><span class="sxs-lookup"><span data-stu-id="35824-117">Select **Suspended**</span></span>

   4. <span data-ttu-id="35824-118">Upprepa dessa steg för varje aktiv prenumeration.</span><span class="sxs-lookup"><span data-stu-id="35824-118">Repeat these steps for each active subscription.</span></span>

2. <span data-ttu-id="35824-119">**Ta bort relationen i Partnercenter:**</span><span class="sxs-lookup"><span data-stu-id="35824-119">**Remove the relationship in Partner Center:**</span></span>

   <span data-ttu-id="35824-120">a.</span><span class="sxs-lookup"><span data-stu-id="35824-120">a.</span></span> <span data-ttu-id="35824-121">Från Partnercenter går du till **Kunder** och väljer en kund.</span><span class="sxs-lookup"><span data-stu-id="35824-121">From the Partner Center, go to **Customers** and select a customer.</span></span>

   <span data-ttu-id="35824-122">b.</span><span class="sxs-lookup"><span data-stu-id="35824-122">b.</span></span> <span data-ttu-id="35824-123">Välj **Konto.**</span><span class="sxs-lookup"><span data-stu-id="35824-123">Select the **Account**.</span></span>

   <span data-ttu-id="35824-124">c.</span><span class="sxs-lookup"><span data-stu-id="35824-124">c.</span></span> <span data-ttu-id="35824-125">Välj **Ta bort återförsäljarrelation.**</span><span class="sxs-lookup"><span data-stu-id="35824-125">Select **Remove reseller relationship**.</span></span>

   > [!NOTE]
   > <span data-ttu-id="35824-126">Om några prenumerationer fortfarande är aktiva kommer länken **Ta bort återförsäljarrelation** att vara inaktiv.</span><span class="sxs-lookup"><span data-stu-id="35824-126">If any subscriptions are still active, the **Remove reseller relationship** link will be inactive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="35824-127">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="35824-127">Next steps</span></span>

- [<span data-ttu-id="35824-128">Begära eller återupprätta en relation med en kund</span><span class="sxs-lookup"><span data-stu-id="35824-128">Request or re-establish a relationship with a customer</span></span>](request-a-relationship-with-a-customer.md)
