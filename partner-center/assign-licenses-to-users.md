---
title: Hantera användare för kundkonton
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hantera användare för dina kunder i Partnercenter – skapa användarkonton, lägga till eller ta bort användarlicenser, återställa lösenord och ta bort eller återställa användarkonton.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149901"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="03041-103">Hantera användare och användarlicenser för kundkonton</span><span class="sxs-lookup"><span data-stu-id="03041-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="03041-104">**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Administratörsagent</span><span class="sxs-lookup"><span data-stu-id="03041-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>


<span data-ttu-id="03041-105">Du kan skapa och ta bort nya användare i en kunds konto.</span><span class="sxs-lookup"><span data-stu-id="03041-105">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="03041-106">Du kan också återställa ett eller flera användarkonton som du tidigare har tagit bort inom 30 dagar efter borttagningen.</span><span class="sxs-lookup"><span data-stu-id="03041-106">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="03041-107">Användarens tidigare prenumerationstilldelningar återställs också (förutsatt att deras tidigare allokeringar är tillgängliga).</span><span class="sxs-lookup"><span data-stu-id="03041-107">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="03041-108">När du köper nya prenumerationer för en kund bör kunden ge dig en lista över alla användare som behöver konton, deras användarbehörigheter och vilka tjänster varje användare behöver.</span><span class="sxs-lookup"><span data-stu-id="03041-108">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="03041-109">Avsnittet **Användare och**  licenser på fliken Kund visar alla användare som skapats i en specifik kunds klientorganisation, inklusive användare som har köpt licenser från en annan CSP-partner eller från en annan inköpskanal.</span><span class="sxs-lookup"><span data-stu-id="03041-109">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="03041-110">Du kan [tilldela prenumerationer till flera användare samtidigt](bulk-license-provisioning-for-multiple-users.md) genom att importera namnen med hjälp av en [Excel-kompatibel CSV-kalkylbladsfil.](adding-multiple-users-to-a-customer-account.md)</span><span class="sxs-lookup"><span data-stu-id="03041-110">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="03041-111">Skapa användarkonton för en kund</span><span class="sxs-lookup"><span data-stu-id="03041-111">Create user accounts for a customer</span></span>

1. <span data-ttu-id="03041-112">Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="03041-112">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="03041-113">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="03041-113">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="03041-114">I kundmenyn väljer du **Användare och licenser.**</span><span class="sxs-lookup"><span data-stu-id="03041-114">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="03041-115">För varje användare som du lägger till **väljer du Lägg** till prenumeration och fyller sedan i informationen, inklusive behörigheter och licenser.</span><span class="sxs-lookup"><span data-stu-id="03041-115">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="03041-116">**Spara** ändringarna.</span><span class="sxs-lookup"><span data-stu-id="03041-116">**Save** your changes.</span></span>

5. <span data-ttu-id="03041-117">Se till att registrera användarnamnet och det tillfälliga lösenordet som ska skickas till användaren.</span><span class="sxs-lookup"><span data-stu-id="03041-117">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="03041-118">Om du lägger till flera användare en i taget använder du Lägg **till en annan användare.**</span><span class="sxs-lookup"><span data-stu-id="03041-118">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="03041-119">Du kan också lägga till flera användare samtidigt genom att [importera en Excel-kompatibel CSV-kalkylbladsfil.](adding-multiple-users-to-a-customer-account.md)</span><span class="sxs-lookup"><span data-stu-id="03041-119">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="03041-120">Du kan vänta tills du är klar med hela uppsättningen innan du skickar e-post eller skriver ut namn och lösenord från bekräftelseskärmen.</span><span class="sxs-lookup"><span data-stu-id="03041-120">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="03041-121">Lägga till eller ta bort användarlicenser för en kund</span><span class="sxs-lookup"><span data-stu-id="03041-121">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="03041-122">Följande steg gäller för att lägga till eller ta bort användarlicenser för Microsoft-produkter.</span><span class="sxs-lookup"><span data-stu-id="03041-122">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="03041-123">Om du vill lägga till eller ta bort användarlicenser för licensbaserade SaaS-prenumerationer på den kommersiella marknadsplatsen kan du läsa Lägga till eller ta bort licenser [för en SaaS-prenumeration.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)</span><span class="sxs-lookup"><span data-stu-id="03041-123">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="03041-124">Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="03041-124">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="03041-125">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="03041-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="03041-126">I kundmenyn väljer du **Användare och licenser.**</span><span class="sxs-lookup"><span data-stu-id="03041-126">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="03041-127">Välj en eller flera användare i listan.</span><span class="sxs-lookup"><span data-stu-id="03041-127">Choose one or more users from the list.</span></span> <span data-ttu-id="03041-128">Om kunden till exempel precis har köpt nya licenser och du vill tilldela dem till personer som inte har dem ännu, kan du använda alternativet **Filtrera användare efter...** för att hitta rätt grupp.</span><span class="sxs-lookup"><span data-stu-id="03041-128">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="03041-129">Välj **Hantera licenser**.</span><span class="sxs-lookup"><span data-stu-id="03041-129">Select **Manage licenses**.</span></span> <span data-ttu-id="03041-130">Gör dina ändringar och sedan **Spara**.</span><span class="sxs-lookup"><span data-stu-id="03041-130">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="03041-131">För [Azure Marketplace produkter](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)hanteras licenstilldelning och aktivering via isv:n (Independent Software Vendor) som publicerade produkten.</span><span class="sxs-lookup"><span data-stu-id="03041-131">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="03041-132">Återställa en användares lösenord för en kund</span><span class="sxs-lookup"><span data-stu-id="03041-132">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="03041-133">Logga in i Partnercenter och gå till [instrumentpanelen](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="03041-133">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="03041-134">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="03041-134">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="03041-135">I kundmenyn väljer du **Användare och licenser.**</span><span class="sxs-lookup"><span data-stu-id="03041-135">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="03041-136">Välj användaren i listan.</span><span class="sxs-lookup"><span data-stu-id="03041-136">Choose the user from the list.</span></span>

4. <span data-ttu-id="03041-137">Längst ned på skärmen väljer du **Återställ lösenord.**</span><span class="sxs-lookup"><span data-stu-id="03041-137">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="03041-138">Skicka det nya tillfälliga lösenordet till användaren.</span><span class="sxs-lookup"><span data-stu-id="03041-138">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="03041-139">Ta bort användarkonton för en kund</span><span class="sxs-lookup"><span data-stu-id="03041-139">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="03041-140">I **menyn i Partnercenter** väljer du **Kunder.**</span><span class="sxs-lookup"><span data-stu-id="03041-140">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="03041-141">Välj kunden i listan.</span><span class="sxs-lookup"><span data-stu-id="03041-141">Choose the customer from the list.</span></span>

2. <span data-ttu-id="03041-142">I kundmenyn väljer du **Användare och licenser.**</span><span class="sxs-lookup"><span data-stu-id="03041-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="03041-143">Välj användaren i listan.</span><span class="sxs-lookup"><span data-stu-id="03041-143">Choose the user from the list.</span></span>

3. <span data-ttu-id="03041-144">Längst ned på skärmen väljer du **Ta bort användarkonto.**</span><span class="sxs-lookup"><span data-stu-id="03041-144">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="03041-145">Om du behöver återställa det här kontot  hittar du det på fliken Borttagna användare i listan Kundens **användare och** licenser.</span><span class="sxs-lookup"><span data-stu-id="03041-145">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="03041-146">Du har 30 dagar på dig att återställa en borttagna användare.</span><span class="sxs-lookup"><span data-stu-id="03041-146">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="03041-147">Återställa borttagna användarkonton</span><span class="sxs-lookup"><span data-stu-id="03041-147">Restore deleted user accounts</span></span>

1. <span data-ttu-id="03041-148">I **menyn i Partnercenter** **väljer du** Kunder och sedan kunden i listan.</span><span class="sxs-lookup"><span data-stu-id="03041-148">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="03041-149">Välj **Användare och licenser.**</span><span class="sxs-lookup"><span data-stu-id="03041-149">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="03041-150">Välj fliken **Borttagna** användare ( ). Den bör läsa **(1)** eller högre när det finns borttagna användare som kan återställas.</span><span class="sxs-lookup"><span data-stu-id="03041-150">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="03041-151">Markera en eller flera av kryssrutorna för borttagna användare och välj sedan **Återställ.**</span><span class="sxs-lookup"><span data-stu-id="03041-151">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="03041-152">Alla valda användarkonton visas igen på sidan **Användare och** licenser.</span><span class="sxs-lookup"><span data-stu-id="03041-152">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="03041-153">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="03041-153">Next steps</span></span>

- [<span data-ttu-id="03041-154">Tilldela eller återkalla licenser till flera användare</span><span class="sxs-lookup"><span data-stu-id="03041-154">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="03041-155">Skapa flera användare för ett kundkonto</span><span class="sxs-lookup"><span data-stu-id="03041-155">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)