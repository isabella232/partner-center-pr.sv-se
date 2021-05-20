---
title: Lägga till flera användare för ett kundkonto
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Om du vill lägga till flera användare till en kunds konto laddar du upp en datafil till Partnercenter med filformatet kommaavgränsade värden (.csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150479"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="c11cd-103">Ladda upp en CSV-fil med användare till en kunds konto</span><span class="sxs-lookup"><span data-stu-id="c11cd-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="c11cd-104">**Lämpliga roller:** Global administratör</span><span class="sxs-lookup"><span data-stu-id="c11cd-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="c11cd-105">Lägg till flera användare till en kunds konto samtidigt genom att ladda upp en datafil i filformatet med kommaavgränsade värden (.csv) till Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="c11cd-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="c11cd-106">Skapa filen med kundanvändare och ladda upp till kundkontot</span><span class="sxs-lookup"><span data-stu-id="c11cd-106">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="c11cd-107">Skapa en datafil med kommaavgränsade värden (.csv) med de data som beskrivs ovan.</span><span class="sxs-lookup"><span data-stu-id="c11cd-107">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="c11cd-108">Spara filen så att du kan bläddra till den i ett senare steg.</span><span class="sxs-lookup"><span data-stu-id="c11cd-108">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="c11cd-109">Se [Fält för CSV-filen för att importera flera användare för ett kundkonto.](file-customer-users.md)</span><span class="sxs-lookup"><span data-stu-id="c11cd-109">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="c11cd-110">Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="c11cd-110">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="c11cd-111">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="c11cd-111">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="c11cd-112">Välj kundens flik **Användare och licenser och** välj sedan Ladda upp **användare.**</span><span class="sxs-lookup"><span data-stu-id="c11cd-112">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="c11cd-113">Under **Ladda upp användarinformation** väljer du **Bläddra**.</span><span class="sxs-lookup"><span data-stu-id="c11cd-113">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="c11cd-114">I filväljaren väljer du din datafil och sedan **Öppna**.</span><span class="sxs-lookup"><span data-stu-id="c11cd-114">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="c11cd-115">Välj **Verifiera**.</span><span class="sxs-lookup"><span data-stu-id="c11cd-115">Select **Validate**.</span></span>

    <span data-ttu-id="c11cd-116">**Obs!**  De flesta fel vid skapande av konton orsakas av problem med datafiler, inklusive information som saknas, felaktiga eller duplicerade e-postadresser eller för många poster i filen.</span><span class="sxs-lookup"><span data-stu-id="c11cd-116">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="c11cd-117">När Partnercenter har verifierat filen väljer du den geografiska **platsen för** de nya användarna.</span><span class="sxs-lookup"><span data-stu-id="c11cd-117">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="c11cd-118">Välj **Spara**.</span><span class="sxs-lookup"><span data-stu-id="c11cd-118">Select **Save**.</span></span>
10. <span data-ttu-id="c11cd-119">Ladda ned den tillfälliga lösenordsinformationen för användarna.</span><span class="sxs-lookup"><span data-stu-id="c11cd-119">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="c11cd-120">Se till att ladda ned filen med de tillfälliga lösenorden nu eftersom du inte kan göra det senare.</span><span class="sxs-lookup"><span data-stu-id="c11cd-120">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="c11cd-121">Nya användare måste logga in på sitt nya konto med det tillfälliga lösenordet för sina nya konton.</span><span class="sxs-lookup"><span data-stu-id="c11cd-121">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="c11cd-122">Nya användare tilldelas automatiskt behörigheter för **Can use licenses and services (Kan använda licenser och tjänster).**</span><span class="sxs-lookup"><span data-stu-id="c11cd-122">New users are automatically assigned permissions of **Can use licenses and services**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="c11cd-123">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="c11cd-123">Next steps</span></span>

- [<span data-ttu-id="c11cd-124">Ge kunderna behörighet i Partnercenter att köpa egna produkter eller tjänster</span><span class="sxs-lookup"><span data-stu-id="c11cd-124">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
