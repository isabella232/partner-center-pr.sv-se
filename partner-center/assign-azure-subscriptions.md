---
title: Tilldela Azure-prenumerationer till kunder
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du tilldelar Azure-prenumerationer till dina kunder i Partner Center och hur du kan göra det möjligt för kunder att hantera sina egna prenumerationer.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8cac2a6edc9199befeae940ed271c3236440c260
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/01/2020
ms.locfileid: "96473959"
---
# <a name="assigning-azure-subscriptions-to-customers-in-partner-center"></a><span data-ttu-id="0a34f-103">Tilldela Azure-prenumerationer till kunder i Partner Center</span><span class="sxs-lookup"><span data-stu-id="0a34f-103">Assigning Azure subscriptions to customers in Partner Center</span></span>

<span data-ttu-id="0a34f-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="0a34f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0a34f-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="0a34f-105">Global admin</span></span>
- <span data-ttu-id="0a34f-106">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="0a34f-106">Sales agent</span></span>

## <a name="assign-azure-subscriptions-to-your-customers"></a><span data-ttu-id="0a34f-107">Tilldela Azure-prenumerationer till dina kunder</span><span class="sxs-lookup"><span data-stu-id="0a34f-107">Assign Azure subscriptions to your customers</span></span>

1. <span data-ttu-id="0a34f-108">Välj **kunder** från menyn **partner Center** och leta upp den kund som du vill hantera.</span><span class="sxs-lookup"><span data-stu-id="0a34f-108">Select **Customers** from your **Partner Center** menu and locate the customer you want to manage.</span></span>

2. <span data-ttu-id="0a34f-109">Välj nedåtpilen i slutet av raden för att expandera kundens post och välj sedan **Microsoft Azure-hanteringsportal**.</span><span class="sxs-lookup"><span data-stu-id="0a34f-109">Select the down arrow at the end of the row to expand the customer's record and then select **Microsoft Azure Management Portal**.</span></span> <span data-ttu-id="0a34f-110">Du dirigeras till [Azure Portal](https://portal.azure.com/) där du kan hantera kundens prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="0a34f-110">You will be directed to the [Azure portal](https://portal.azure.com/) where you can manage the customer's subscriptions.</span></span>

3. <span data-ttu-id="0a34f-111">Välj **prenumerationer** från Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="0a34f-111">From the Azure portal, select **Subscriptions**.</span></span>

4. <span data-ttu-id="0a34f-112">Välj den prenumeration som du vill tilldela och välj **Access Control**.</span><span class="sxs-lookup"><span data-stu-id="0a34f-112">Select the subscription you would like to assign, then select **Access Control**.</span></span>

5. <span data-ttu-id="0a34f-113">Välj **Lägg till** för att lägga till en användare i prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="0a34f-113">Select **Add** to add a user to the subscription.</span></span> 

6. <span data-ttu-id="0a34f-114">När du har lagt till användaren i prenumerationen kan du tilldela användaren en roll och det angivna kontot som användaren kommer att ha åtkomst till.</span><span class="sxs-lookup"><span data-stu-id="0a34f-114">After you add the user to the subscription, you can assign the user a role and the specific account that user will have access to.</span></span>

## <a name="enable-customers-to-manage-their-azure-subscriptions"></a><span data-ttu-id="0a34f-115">Gör det möjligt för kunder att hantera sina Azure-prenumerationer</span><span class="sxs-lookup"><span data-stu-id="0a34f-115">Enable customers to manage their Azure subscriptions</span></span>

<span data-ttu-id="0a34f-116">När du har skapat en Microsoft Azure-prenumeration för en kund kan du göra det möjligt för dem att hantera prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="0a34f-116">After you create a Microsoft Azure subscription for a customer, you can enable them to manage the subscription.</span></span> <span data-ttu-id="0a34f-117">För att göra detta måste du logga in på kundens Microsoft Azure hanterings Portal.</span><span class="sxs-lookup"><span data-stu-id="0a34f-117">To do this, you'll need to log on to the customer's Microsoft Azure Management portal.</span></span> 

1. <span data-ttu-id="0a34f-118">Öppna kundens Azure Portal genom att antingen expandera kundens lista i din kund lista eller Välj kundens namn och välj sedan **Microsoft Azure-hanteringsportal**.</span><span class="sxs-lookup"><span data-stu-id="0a34f-118">To open the customer's Azure portal, either expand the customer's listing in your customer list or select the customer's name and then select **Microsoft Azure Management Portal**.</span></span>

   > [!NOTE]  
   > <span data-ttu-id="0a34f-119">Om du uppmanas att logga in på Azure Portal kanske du inte har delegerad administratörs behörighet.</span><span class="sxs-lookup"><span data-stu-id="0a34f-119">If you are prompted to log onto the Azure portal, you may not have delegated administrative privileges.</span></span> <span data-ttu-id="0a34f-120">Välj **begär en relation** för att bjuda in kunden att identifiera dig som sin partner av posten.</span><span class="sxs-lookup"><span data-stu-id="0a34f-120">Select **Request a relationship** to invite the customer to identify you as their Partner of Record.</span></span> <span data-ttu-id="0a34f-121">När kunden har accepterat din inbjudan beviljas du automatiskt delegerad administratörs behörighet.</span><span class="sxs-lookup"><span data-stu-id="0a34f-121">After the customer accepts your invitation, you are automatically granted delegated administrative privileges.</span></span>

2. <span data-ttu-id="0a34f-122">I Azure Portal öppnar du kund prenumerations listan och väljer kundens Azure-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="0a34f-122">In the Azure portal, open the customer's subscriptions list and select the customer's Azure subscription.</span></span>

3. <span data-ttu-id="0a34f-123">Tilldela en roll till någon av kundens användare så att de kan skapa och hantera resurser under prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="0a34f-123">Assign a role to any of the customer's users so that they can create and manage resources under their subscription.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0a34f-124">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="0a34f-124">Next steps</span></span>

- [<span data-ttu-id="0a34f-125">Hur CSP-partner kan sälja prenumerationer till kunder</span><span class="sxs-lookup"><span data-stu-id="0a34f-125">How CSP partners can sell subscriptions to customers</span></span>](customer-subscriptions.md)

- [<span data-ttu-id="0a34f-126">Så här hämtar du behörigheter för att hantera en kunds tjänst eller prenumerationer</span><span class="sxs-lookup"><span data-stu-id="0a34f-126">How to obtain permissions to manage a customer's service or subscriptions</span></span>](customers-revoke-admin-privileges.md)
