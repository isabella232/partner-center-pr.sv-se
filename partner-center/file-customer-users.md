---
title: Fält för. csv-fil för att importera flera användare för ett kund konto
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Om du vill lägga till flera användare i ett kund konto skapar du en fil med kommaavgränsade värden (. csv) med lämpliga fält.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441429"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="b66e7-103">Lägg till flera användare till ett kund konto genom att skapa en. csv-fil</span><span class="sxs-lookup"><span data-stu-id="b66e7-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="b66e7-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="b66e7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b66e7-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="b66e7-105">Global admin</span></span>

<span data-ttu-id="b66e7-106">Lägg till flera användare till ett kund konto samtidigt, genom att ladda upp en datafil i det kommaavgränsade värde fil formatet (. csv) till Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b66e7-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="b66e7-107">Du kan ladda ned en exempel data fil från Partner Center och sedan redigera den för din användning, eller så kan du skapa en ny datafil med hjälp av den data modell som anges nedan.</span><span class="sxs-lookup"><span data-stu-id="b66e7-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="b66e7-108">Krav för data fil</span><span class="sxs-lookup"><span data-stu-id="b66e7-108">Data file requirements</span></span>

<span data-ttu-id="b66e7-109">Om du vill lägga till flera användare till ett kund konto med processen för Mass uppladdning måste du uppfylla följande krav:</span><span class="sxs-lookup"><span data-stu-id="b66e7-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="b66e7-110">Du måste ha global administratörs behörighet till kund kontot.</span><span class="sxs-lookup"><span data-stu-id="b66e7-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="b66e7-111">Varje användare måste ha en unik e-postadress som läggs till kundens e-postdomän.</span><span class="sxs-lookup"><span data-stu-id="b66e7-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="b66e7-112">Du kan ladda upp upp till 100 poster i taget.</span><span class="sxs-lookup"><span data-stu-id="b66e7-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="b66e7-113">Om du behöver lägga till fler än 100 användare skapar du och laddar upp ytterligare datafiler.</span><span class="sxs-lookup"><span data-stu-id="b66e7-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="b66e7-114">Alla användare måste finnas på samma geografiska **plats**.</span><span class="sxs-lookup"><span data-stu-id="b66e7-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="b66e7-115">Ange endast de data som beskrivs nedan.</span><span class="sxs-lookup"><span data-stu-id="b66e7-115">Enter only the data described below.</span></span> <span data-ttu-id="b66e7-116">Främmande data gör att överföringen Miss fungerar.</span><span class="sxs-lookup"><span data-stu-id="b66e7-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="b66e7-117">Ange följande data i data filen:</span><span class="sxs-lookup"><span data-stu-id="b66e7-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="b66e7-118">**Kolumnnamn**</span><span class="sxs-lookup"><span data-stu-id="b66e7-118">**Column name**</span></span> | <span data-ttu-id="b66e7-119">**Beskrivning**</span><span class="sxs-lookup"><span data-stu-id="b66e7-119">**Description**</span></span>  | <span data-ttu-id="b66e7-120">**Begränsning**</span><span class="sxs-lookup"><span data-stu-id="b66e7-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="b66e7-121">Förnamn</span><span class="sxs-lookup"><span data-stu-id="b66e7-121">First name</span></span>  | <span data-ttu-id="b66e7-122">Användarens förnamn (valfritt fält)</span><span class="sxs-lookup"><span data-stu-id="b66e7-122">User's first name (optional field)</span></span>  | <span data-ttu-id="b66e7-123">50 – tecken gräns</span><span class="sxs-lookup"><span data-stu-id="b66e7-123">50-character limit</span></span>  |
| <span data-ttu-id="b66e7-124">Efternamn</span><span class="sxs-lookup"><span data-stu-id="b66e7-124">Last name</span></span>  | <span data-ttu-id="b66e7-125">Användarens efter namn (valfritt fält)</span><span class="sxs-lookup"><span data-stu-id="b66e7-125">User's last name (optional field)</span></span>  | <span data-ttu-id="b66e7-126">50 – tecken gräns</span><span class="sxs-lookup"><span data-stu-id="b66e7-126">50-character limit</span></span>  |
| <span data-ttu-id="b66e7-127">Visningsnamn</span><span class="sxs-lookup"><span data-stu-id="b66e7-127">Display name</span></span>    | <span data-ttu-id="b66e7-128">Namn som visas i Partner Center (obligatoriskt fält)</span><span class="sxs-lookup"><span data-stu-id="b66e7-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="b66e7-129">50 – tecken gräns</span><span class="sxs-lookup"><span data-stu-id="b66e7-129">50-character limit</span></span>                         |
| <span data-ttu-id="b66e7-130">E-post</span><span class="sxs-lookup"><span data-stu-id="b66e7-130">Email</span></span>   | <span data-ttu-id="b66e7-131">Användarens företags-e-postadress på kund företaget (obligatoriskt fält)</span><span class="sxs-lookup"><span data-stu-id="b66e7-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="b66e7-132">Varje användare måste ha en unik e-postadress</span><span class="sxs-lookup"><span data-stu-id="b66e7-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="b66e7-133">Status uppdatering</span><span class="sxs-lookup"><span data-stu-id="b66e7-133">Status update</span></span>   | <span data-ttu-id="b66e7-134">Används för att ange om den nya användar posten har skapats</span><span class="sxs-lookup"><span data-stu-id="b66e7-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="b66e7-135">\*\*Lämna tomt\*\*</span><span class="sxs-lookup"><span data-stu-id="b66e7-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="b66e7-136">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="b66e7-136">Next steps</span></span>

- [<span data-ttu-id="b66e7-137">Så här lägger du till flera användare för en kund</span><span class="sxs-lookup"><span data-stu-id="b66e7-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)