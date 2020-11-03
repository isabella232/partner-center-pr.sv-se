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
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/03/2020
ms.locfileid: "92531160"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="9bae2-103">Lägg till flera användare till ett kund konto genom att skapa en. csv-fil</span><span class="sxs-lookup"><span data-stu-id="9bae2-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="9bae2-104">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="9bae2-104">**Applies to**</span></span>

- <span data-ttu-id="9bae2-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="9bae2-105">Partner Center</span></span>

<span data-ttu-id="9bae2-106">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="9bae2-106">**Appropriate roles**</span></span>

- <span data-ttu-id="9bae2-107">Global administratör</span><span class="sxs-lookup"><span data-stu-id="9bae2-107">Global admin</span></span>

<span data-ttu-id="9bae2-108">Lägg till flera användare till ett kund konto samtidigt, genom att ladda upp en datafil i det kommaavgränsade värde fil formatet (. csv) till Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9bae2-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="9bae2-109">Du kan ladda ned en exempel data fil från Partner Center och sedan redigera den för din användning, eller så kan du skapa en ny datafil med hjälp av den data modell som anges nedan.</span><span class="sxs-lookup"><span data-stu-id="9bae2-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="9bae2-110">Krav för data fil</span><span class="sxs-lookup"><span data-stu-id="9bae2-110">Data file requirements</span></span>

<span data-ttu-id="9bae2-111">Om du vill lägga till flera användare till ett kund konto med processen för Mass uppladdning måste du uppfylla följande krav:</span><span class="sxs-lookup"><span data-stu-id="9bae2-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="9bae2-112">Du måste ha global administratörs behörighet till kund kontot.</span><span class="sxs-lookup"><span data-stu-id="9bae2-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="9bae2-113">Varje användare måste ha en unik e-postadress som läggs till kundens e-postdomän.</span><span class="sxs-lookup"><span data-stu-id="9bae2-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="9bae2-114">Du kan ladda upp upp till 100 poster i taget.</span><span class="sxs-lookup"><span data-stu-id="9bae2-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="9bae2-115">Om du behöver lägga till fler än 100 användare skapar du och laddar upp ytterligare datafiler.</span><span class="sxs-lookup"><span data-stu-id="9bae2-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="9bae2-116">Alla användare måste finnas på samma geografiska **plats** .</span><span class="sxs-lookup"><span data-stu-id="9bae2-116">All users must be in the same geographic **Location** .</span></span>
- <span data-ttu-id="9bae2-117">Ange endast de data som beskrivs nedan.</span><span class="sxs-lookup"><span data-stu-id="9bae2-117">Enter only the data described below.</span></span> <span data-ttu-id="9bae2-118">Främmande data gör att överföringen Miss fungerar.</span><span class="sxs-lookup"><span data-stu-id="9bae2-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="9bae2-119">Ange följande data i data filen:</span><span class="sxs-lookup"><span data-stu-id="9bae2-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="9bae2-120">**Kolumnnamn**</span><span class="sxs-lookup"><span data-stu-id="9bae2-120">**Column name**</span></span> | <span data-ttu-id="9bae2-121">**Beskrivning**</span><span class="sxs-lookup"><span data-stu-id="9bae2-121">**Description**</span></span>  | <span data-ttu-id="9bae2-122">**Begränsning**</span><span class="sxs-lookup"><span data-stu-id="9bae2-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="9bae2-123">Förnamn</span><span class="sxs-lookup"><span data-stu-id="9bae2-123">First name</span></span>  | <span data-ttu-id="9bae2-124">Användarens förnamn (valfritt fält)</span><span class="sxs-lookup"><span data-stu-id="9bae2-124">User's first name (optional field)</span></span>  | <span data-ttu-id="9bae2-125">50 – tecken gräns</span><span class="sxs-lookup"><span data-stu-id="9bae2-125">50-character limit</span></span>  |
| <span data-ttu-id="9bae2-126">Efternamn</span><span class="sxs-lookup"><span data-stu-id="9bae2-126">Last name</span></span>  | <span data-ttu-id="9bae2-127">Användarens efter namn (valfritt fält)</span><span class="sxs-lookup"><span data-stu-id="9bae2-127">User's last name (optional field)</span></span>  | <span data-ttu-id="9bae2-128">50 – tecken gräns</span><span class="sxs-lookup"><span data-stu-id="9bae2-128">50-character limit</span></span>  |
| <span data-ttu-id="9bae2-129">Visningsnamn</span><span class="sxs-lookup"><span data-stu-id="9bae2-129">Display name</span></span>    | <span data-ttu-id="9bae2-130">Namn som visas i Partner Center (obligatoriskt fält)</span><span class="sxs-lookup"><span data-stu-id="9bae2-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="9bae2-131">50 – tecken gräns</span><span class="sxs-lookup"><span data-stu-id="9bae2-131">50-character limit</span></span>                         |
| <span data-ttu-id="9bae2-132">E-post</span><span class="sxs-lookup"><span data-stu-id="9bae2-132">Email</span></span>   | <span data-ttu-id="9bae2-133">Användarens företags-e-postadress på kund företaget (obligatoriskt fält)</span><span class="sxs-lookup"><span data-stu-id="9bae2-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="9bae2-134">Varje användare måste ha en unik e-postadress</span><span class="sxs-lookup"><span data-stu-id="9bae2-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="9bae2-135">Status uppdatering</span><span class="sxs-lookup"><span data-stu-id="9bae2-135">Status update</span></span>   | <span data-ttu-id="9bae2-136">Används för att ange om den nya användar posten har skapats eller inte</span><span class="sxs-lookup"><span data-stu-id="9bae2-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="9bae2-137">\*\*Lämna tomt\*\*</span><span class="sxs-lookup"><span data-stu-id="9bae2-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="9bae2-138">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="9bae2-138">Next steps</span></span>

- [<span data-ttu-id="9bae2-139">Så här lägger du till flera användare för en kund</span><span class="sxs-lookup"><span data-stu-id="9bae2-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)