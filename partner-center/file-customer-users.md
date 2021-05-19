---
title: Fält för CSV-fil för att importera flera användare för ett kundkonto
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Om du vill lägga till flera användare till ett kundkonto skapar du en fil med kommaavgränsade värden (.csv) med lämpliga fält.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150989"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="8a92c-103">Lägga till flera användare till ett kundkonto genom att skapa en CSV-fil</span><span class="sxs-lookup"><span data-stu-id="8a92c-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="8a92c-104">**Lämpliga roller:** Global administratör</span><span class="sxs-lookup"><span data-stu-id="8a92c-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="8a92c-105">Lägg till flera användare till en kunds konto samtidigt genom att ladda upp en datafil i filformatet med kommaavgränsade värden (.csv) till Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="8a92c-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="8a92c-106">Du kan ladda ned en exempeldatafil från Partnercenter och sedan redigera den för din användning, eller så kan du skapa en ny datafil med hjälp av den datamodell som definieras nedan.</span><span class="sxs-lookup"><span data-stu-id="8a92c-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="8a92c-107">Krav för datafiler</span><span class="sxs-lookup"><span data-stu-id="8a92c-107">Data file requirements</span></span>

<span data-ttu-id="8a92c-108">Om du vill lägga till flera användare till en kunds konto med massuppladdningsprocessen måste du uppfylla följande krav:</span><span class="sxs-lookup"><span data-stu-id="8a92c-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="8a92c-109">Du måste ha behörighet som global administratör för kundkontot.</span><span class="sxs-lookup"><span data-stu-id="8a92c-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="8a92c-110">Varje användare måste ha en unik e-postadress som läggs till i kundens e-postdomäner;</span><span class="sxs-lookup"><span data-stu-id="8a92c-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="8a92c-111">Du kan ladda upp upp till 100 poster i taget.</span><span class="sxs-lookup"><span data-stu-id="8a92c-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="8a92c-112">Om du behöver lägga till fler än 100 användare kan du skapa och ladda upp ytterligare datafiler.</span><span class="sxs-lookup"><span data-stu-id="8a92c-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="8a92c-113">Alla användare måste finnas på samma geografiska **plats.**</span><span class="sxs-lookup"><span data-stu-id="8a92c-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="8a92c-114">Ange endast de data som beskrivs nedan.</span><span class="sxs-lookup"><span data-stu-id="8a92c-114">Enter only the data described below.</span></span> <span data-ttu-id="8a92c-115">Överflödiga data gör att uppladdningen misslyckas.</span><span class="sxs-lookup"><span data-stu-id="8a92c-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="8a92c-116">Ange följande data i datafilen:</span><span class="sxs-lookup"><span data-stu-id="8a92c-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="8a92c-117">**Kolumnnamn**</span><span class="sxs-lookup"><span data-stu-id="8a92c-117">**Column name**</span></span> | <span data-ttu-id="8a92c-118">**Beskrivning**</span><span class="sxs-lookup"><span data-stu-id="8a92c-118">**Description**</span></span>  | <span data-ttu-id="8a92c-119">**Begränsning**</span><span class="sxs-lookup"><span data-stu-id="8a92c-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="8a92c-120">Förnamn</span><span class="sxs-lookup"><span data-stu-id="8a92c-120">First name</span></span>  | <span data-ttu-id="8a92c-121">Användarens förnamn (valfritt fält)</span><span class="sxs-lookup"><span data-stu-id="8a92c-121">User's first name (optional field)</span></span>  | <span data-ttu-id="8a92c-122">Gräns på 50 tecken</span><span class="sxs-lookup"><span data-stu-id="8a92c-122">50-character limit</span></span>  |
| <span data-ttu-id="8a92c-123">Efternamn</span><span class="sxs-lookup"><span data-stu-id="8a92c-123">Last name</span></span>  | <span data-ttu-id="8a92c-124">Användarens efternamn (valfritt fält)</span><span class="sxs-lookup"><span data-stu-id="8a92c-124">User's last name (optional field)</span></span>  | <span data-ttu-id="8a92c-125">Gräns på 50 tecken</span><span class="sxs-lookup"><span data-stu-id="8a92c-125">50-character limit</span></span>  |
| <span data-ttu-id="8a92c-126">Visningsnamn</span><span class="sxs-lookup"><span data-stu-id="8a92c-126">Display name</span></span>    | <span data-ttu-id="8a92c-127">Namn som visas i Partnercenter (obligatoriskt fält)</span><span class="sxs-lookup"><span data-stu-id="8a92c-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="8a92c-128">Gräns på 50 tecken</span><span class="sxs-lookup"><span data-stu-id="8a92c-128">50-character limit</span></span>                         |
| <span data-ttu-id="8a92c-129">E-post</span><span class="sxs-lookup"><span data-stu-id="8a92c-129">Email</span></span>   | <span data-ttu-id="8a92c-130">Användarens företags-e-postadress på kundföretaget (obligatoriskt fält)</span><span class="sxs-lookup"><span data-stu-id="8a92c-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="8a92c-131">Varje användare måste ha en unik e-postadress</span><span class="sxs-lookup"><span data-stu-id="8a92c-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="8a92c-132">Statusuppdatering</span><span class="sxs-lookup"><span data-stu-id="8a92c-132">Status update</span></span>   | <span data-ttu-id="8a92c-133">Används för att ange om den nya användarposten har skapats</span><span class="sxs-lookup"><span data-stu-id="8a92c-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="8a92c-134">\*\*Lämna tomt\*\*</span><span class="sxs-lookup"><span data-stu-id="8a92c-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="8a92c-135">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="8a92c-135">Next steps</span></span>

- [<span data-ttu-id="8a92c-136">Så här lägger du till flera användare för en kund</span><span class="sxs-lookup"><span data-stu-id="8a92c-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)