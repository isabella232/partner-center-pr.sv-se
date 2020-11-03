---
title: Hantera användare och användar licenser för kund konton
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du hanterar användare för dina kunder i Partner Center, till exempel skapa användar konton, lägga till eller ta bort användar licenser, återställa användar lösen ord och ta bort eller återställa användar konton.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fc208283e0ed8c0f164a44cc9bd70260b8671c6e
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532105"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="18092-103">Hantera användare och användar licenser för kund konton</span><span class="sxs-lookup"><span data-stu-id="18092-103">Manage users and user licenses for customer accounts</span></span>

<span data-ttu-id="18092-104">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="18092-104">**Applies to**</span></span>

- <span data-ttu-id="18092-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="18092-105">Partner Center</span></span>

<span data-ttu-id="18092-106">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="18092-106">**Appropriate roles**</span></span>

- <span data-ttu-id="18092-107">Global administratör</span><span class="sxs-lookup"><span data-stu-id="18092-107">Global admin</span></span>
- <span data-ttu-id="18092-108">Administratör för användar hantering</span><span class="sxs-lookup"><span data-stu-id="18092-108">User management admin</span></span>
- <span data-ttu-id="18092-109">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="18092-109">Admin agent</span></span>
- <span data-ttu-id="18092-110">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="18092-110">Sales agent</span></span>
- <span data-ttu-id="18092-111">Support agent</span><span class="sxs-lookup"><span data-stu-id="18092-111">Helpdesk agent</span></span>

<span data-ttu-id="18092-112">Du kan skapa och ta bort nya användare i ett kund konto.</span><span class="sxs-lookup"><span data-stu-id="18092-112">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="18092-113">Du kan också återställa ett eller flera användar konton som du tidigare tog bort inom 30 dagar från borttagningen.</span><span class="sxs-lookup"><span data-stu-id="18092-113">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="18092-114">Användarens tidigare prenumerations tilldelningar återställs också (förutsatt att deras tidigare allokeringar är tillgängliga).</span><span class="sxs-lookup"><span data-stu-id="18092-114">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="18092-115">När du köper nya prenumerationer för en kund bör kunden ge dig en lista över alla användare som behöver konton, deras användar behörigheter och vilka tjänster varje användare behöver.</span><span class="sxs-lookup"><span data-stu-id="18092-115">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="18092-116">Du kan [tilldela prenumerationer till flera användare](bulk-license-provisioning-for-multiple-users.md) i taget genom att importera namnen med en [Excel-kompatibel. csv-kalkylbladsfilen](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="18092-116">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="18092-117">Skapa användar konton för en kund</span><span class="sxs-lookup"><span data-stu-id="18092-117">Create user accounts for a customer</span></span>

1. <span data-ttu-id="18092-118">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.</span><span class="sxs-lookup"><span data-stu-id="18092-118">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="18092-119">Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="18092-119">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="18092-120">I menyn kund väljer **du användare och licenser** .</span><span class="sxs-lookup"><span data-stu-id="18092-120">In the customer menu, select **Users and licenses** .</span></span>

4. <span data-ttu-id="18092-121">För varje användare som du lägger till väljer du **Lägg till prenumeration** och fyller sedan i informationen, inklusive behörigheter och licenser.</span><span class="sxs-lookup"><span data-stu-id="18092-121">For each user you add, select **Add subscription** , then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="18092-122">**Spara** ändringarna.</span><span class="sxs-lookup"><span data-stu-id="18092-122">**Save** your changes.</span></span>

5. <span data-ttu-id="18092-123">Se till att du registrerar användar namnet och det tillfälliga lösen ordet för att skicka till användaren.</span><span class="sxs-lookup"><span data-stu-id="18092-123">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="18092-124">Om du lägger till flera användare en i taget använder du **Lägg till en annan användare** .</span><span class="sxs-lookup"><span data-stu-id="18092-124">If you are adding multiple users one at a time use **Add another user** .</span></span>

7. <span data-ttu-id="18092-125">Du kan också lägga till flera användare samtidigt genom att [Importera en Excel-kompatibel. csv-kalkylbladsfilen](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="18092-125">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="18092-126">Du kan vänta tills du är klar med hela uppsättningen innan du skickar eller skriver ut namn och lösen ord från bekräftelse skärmen.</span><span class="sxs-lookup"><span data-stu-id="18092-126">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="18092-127">Lägga till eller ta bort användar licenser för en kund</span><span class="sxs-lookup"><span data-stu-id="18092-127">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="18092-128">Följande steg gäller för att lägga till eller ta bort användar licenser för Microsoft-produkter.</span><span class="sxs-lookup"><span data-stu-id="18092-128">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="18092-129">Om du vill lägga till eller ta bort användar licenser för licensbaserade SaaS-prenumerationer på den kommersiella Marketplace, se [lägga till eller ta bort licenser för en SaaS-prenumeration](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="18092-129">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="18092-130">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.</span><span class="sxs-lookup"><span data-stu-id="18092-130">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="18092-131">Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="18092-131">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="18092-132">I menyn kund väljer **du användare och licenser** .</span><span class="sxs-lookup"><span data-stu-id="18092-132">In the customer menu, select **Users and licenses** .</span></span>

4. <span data-ttu-id="18092-133">Välj en eller flera användare i listan.</span><span class="sxs-lookup"><span data-stu-id="18092-133">Choose one or more users from the list.</span></span> <span data-ttu-id="18092-134">Om kunden till exempel precis har köpt nya licenser och du vill tilldela dem till personer som inte har dem än kan du använda alternativet **filtrera användare efter...** för att hitta rätt grupp.</span><span class="sxs-lookup"><span data-stu-id="18092-134">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="18092-135">Välj **Hantera licenser** .</span><span class="sxs-lookup"><span data-stu-id="18092-135">Select **Manage licenses** .</span></span> <span data-ttu-id="18092-136">Gör dina ändringar och **Spara** sedan.</span><span class="sxs-lookup"><span data-stu-id="18092-136">Make your changes, then **Save** .</span></span>

> [!NOTE]
> <span data-ttu-id="18092-137">För [Azure Marketplace-produkter](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)hanteras licens tilldelning och aktivering via den oberoende program varu leverantör (ISV) som publicerade produkten.</span><span class="sxs-lookup"><span data-stu-id="18092-137">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="18092-138">Återställa en användares lösen ord för en kund</span><span class="sxs-lookup"><span data-stu-id="18092-138">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="18092-139">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.</span><span class="sxs-lookup"><span data-stu-id="18092-139">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="18092-140">Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="18092-140">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3.  <span data-ttu-id="18092-141">I menyn kund väljer **du användare och licenser** .</span><span class="sxs-lookup"><span data-stu-id="18092-141">In the customer menu, select **Users and licenses** .</span></span> <span data-ttu-id="18092-142">Välj användaren i listan.</span><span class="sxs-lookup"><span data-stu-id="18092-142">Choose the user from the list.</span></span>

4.  <span data-ttu-id="18092-143">Längst ned på skärmen väljer du **Återställ lösen ord** .</span><span class="sxs-lookup"><span data-stu-id="18092-143">At the bottom of the screen, select **Reset password** .</span></span> 

5.  <span data-ttu-id="18092-144">Skicka det nya tillfälliga lösen ordet till användaren.</span><span class="sxs-lookup"><span data-stu-id="18092-144">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="18092-145">Ta bort användar konton för en kund</span><span class="sxs-lookup"><span data-stu-id="18092-145">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="18092-146">Från menyn **partner Center** väljer du **kunder** .</span><span class="sxs-lookup"><span data-stu-id="18092-146">From the **Partner Center** menu, select **Customers** .</span></span> <span data-ttu-id="18092-147">Välj kund i listan.</span><span class="sxs-lookup"><span data-stu-id="18092-147">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="18092-148">I menyn kund väljer **du användare och licenser** .</span><span class="sxs-lookup"><span data-stu-id="18092-148">In the customer menu, select **Users and licenses** .</span></span> <span data-ttu-id="18092-149">Välj användaren i listan.</span><span class="sxs-lookup"><span data-stu-id="18092-149">Choose the user from the list.</span></span>

3.  <span data-ttu-id="18092-150">Längst ned på skärmen väljer du **ta bort användar konto** .</span><span class="sxs-lookup"><span data-stu-id="18092-150">At the bottom of the screen, select **Delete user account** .</span></span>

<span data-ttu-id="18092-151">Om du behöver återställa det här kontot kan du hitta det på fliken **borttagna användare** i listan kund **användare och licenser** .</span><span class="sxs-lookup"><span data-stu-id="18092-151">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="18092-152">Du har 30 dagar på dig att återställa en borttagen användare.</span><span class="sxs-lookup"><span data-stu-id="18092-152">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="18092-153">Återställa borttagna användar konton</span><span class="sxs-lookup"><span data-stu-id="18092-153">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="18092-154">Från menyn **partner Center** väljer du **kunder** och väljer sedan kunden i listan.</span><span class="sxs-lookup"><span data-stu-id="18092-154">From the **Partner Center** menu, select **Customers** , then choose the customer from the list.</span></span>

2.  <span data-ttu-id="18092-155">Välj **användare och licenser** .</span><span class="sxs-lookup"><span data-stu-id="18092-155">Select **Users and licenses** .</span></span>

3.  <span data-ttu-id="18092-156">Välj fliken **borttagna användare ()** . Den bör läsa **(1)** eller större när det finns borttagna användare som kan återställas.</span><span class="sxs-lookup"><span data-stu-id="18092-156">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="18092-157">Välj en eller flera av kryss rutorna för borttagna användare och välj sedan **Återställ** .</span><span class="sxs-lookup"><span data-stu-id="18092-157">Select one or more of the deleted users' checkboxes and then select **Restore** .</span></span>

    <span data-ttu-id="18092-158">Alla valda användar konton kommer att visas på sidan **användare och licenser** .</span><span class="sxs-lookup"><span data-stu-id="18092-158">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="18092-159">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="18092-159">Related topics</span></span>


[<span data-ttu-id="18092-160">Tilldela eller återkalla licenser till flera användare</span><span class="sxs-lookup"><span data-stu-id="18092-160">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="18092-161">Skapa flera användare för ett kund konto</span><span class="sxs-lookup"><span data-stu-id="18092-161">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)