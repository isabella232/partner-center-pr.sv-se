---
title: Få insikter med kund aktivitets loggar
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du visar och exporterar aktivitets loggar för att få insikt om kund konto transaktioner och andra kund relaterade aktiviteter för partner hantering.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1eaa7fee628015eb633cac3a2796e371f6046585
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474248"
---
# <a name="view-or-export-customer-activity-logs-for-more-insight-into-customer-transactions"></a><span data-ttu-id="0bc40-103">Visa eller exportera kund aktivitets loggar för mer insikter om kund transaktioner</span><span class="sxs-lookup"><span data-stu-id="0bc40-103">View or export customer activity logs for more insight into customer transactions</span></span>

<span data-ttu-id="0bc40-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="0bc40-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0bc40-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="0bc40-105">Global admin</span></span>
- <span data-ttu-id="0bc40-106">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="0bc40-106">Billing admin</span></span>
- <span data-ttu-id="0bc40-107">Administratör för användar hantering</span><span class="sxs-lookup"><span data-stu-id="0bc40-107">User management admin</span></span>
- <span data-ttu-id="0bc40-108">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="0bc40-108">Admin agent</span></span>
- <span data-ttu-id="0bc40-109">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="0bc40-109">Sales agent</span></span>
- <span data-ttu-id="0bc40-110">Support agent</span><span class="sxs-lookup"><span data-stu-id="0bc40-110">Helpdesk agent</span></span>

<span data-ttu-id="0bc40-111">Aktivitets loggar innehåller information om transaktioner och partner hanterings åtgärder för kunder.</span><span class="sxs-lookup"><span data-stu-id="0bc40-111">Activity logs provide information on transactions and Partner management actions for customers.</span></span> <span data-ttu-id="0bc40-112">Loggar för transaktioner ger detaljerad information om transaktionen, inklusive köpta prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="0bc40-112">Logs for transactions provide detailed information about the transaction, including purchased subscriptions.</span></span> <span data-ttu-id="0bc40-113">Du kan också exportera aktivitets loggar till ett Excel-kompatibelt kommaavgränsat värde fil format (. csv).</span><span class="sxs-lookup"><span data-stu-id="0bc40-113">You can also export activity logs to an Excel-compatible comma-separated value file format (.csv).</span></span>

<span data-ttu-id="0bc40-114">Aktivitets loggar innehåller poster för partner åtgärder på kund konton och produkt transaktioner.</span><span class="sxs-lookup"><span data-stu-id="0bc40-114">Activity logs provide records for Partner actions on customer accounts and product transactions.</span></span> <span data-ttu-id="0bc40-115">Du kan också exportera aktivitets loggar till en. csv-fil.</span><span class="sxs-lookup"><span data-stu-id="0bc40-115">You can also export activity logs to a .csv file.</span></span>

## <a name="view-and-export-activity-logs"></a><span data-ttu-id="0bc40-116">Visa och exportera aktivitets loggar</span><span class="sxs-lookup"><span data-stu-id="0bc40-116">View and export activity logs</span></span>

1. <span data-ttu-id="0bc40-117">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.</span><span class="sxs-lookup"><span data-stu-id="0bc40-117">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="0bc40-118">Från menyn **konto inställningar** väljer du **aktivitets logg**.</span><span class="sxs-lookup"><span data-stu-id="0bc40-118">From the **Account settings** menu, select **Activity Log**.</span></span>

3. <span data-ttu-id="0bc40-119">Välj aktivitets logg perioden i fälten **från** och **till** .</span><span class="sxs-lookup"><span data-stu-id="0bc40-119">Select the activity log period in the **From** and **to** fields.</span></span> <span data-ttu-id="0bc40-120">Aktivitets logg exportens standardinställningar är den senaste månaden.</span><span class="sxs-lookup"><span data-stu-id="0bc40-120">The activity log export defaults to the most recent month.</span></span>

   <span data-ttu-id="0bc40-121">Varje aktivitets logg innehåller en länk till kund **prenumerations** sidan.</span><span class="sxs-lookup"><span data-stu-id="0bc40-121">Each activity log provides a link to the listed customer's **Subscriptions** page.</span></span>

   <span data-ttu-id="0bc40-122">Välj en nedåtpil för aktivitets loggen om du vill visa information om en loggad åtgärd.</span><span class="sxs-lookup"><span data-stu-id="0bc40-122">Select a down arrow for any activity log to view details about a logged action.</span></span> <span data-ttu-id="0bc40-123">En enda aktivitets logg kan visa en stor mängd data, till exempel sortering av flera produkter.</span><span class="sxs-lookup"><span data-stu-id="0bc40-123">A single activity log can show a significant amount of data, such as the ordering of multiple products.</span></span>

4. <span data-ttu-id="0bc40-124">Data kolumnerna i loggen innehåller följande:</span><span class="sxs-lookup"><span data-stu-id="0bc40-124">The data columns of the log include the following:</span></span>
   - <span data-ttu-id="0bc40-125">**Datum/tid**-datum och tid för åtgärden.</span><span class="sxs-lookup"><span data-stu-id="0bc40-125">**Date-Time**-the date and time of the action;</span></span>
   - <span data-ttu-id="0bc40-126">**Berörd kund**– kundens företags namn;</span><span class="sxs-lookup"><span data-stu-id="0bc40-126">**Affected customer**—the customer's company name;</span></span>
   - <span data-ttu-id="0bc40-127">**Åtgärd**– åtgärden som vidtas av kunden, till exempel "skapa en hänvisning";</span><span class="sxs-lookup"><span data-stu-id="0bc40-127">**Action**—the action taken by the customer such as "created a referral";</span></span>
   - <span data-ttu-id="0bc40-128">**Partner användare**– partnern som är kopplad till aktiviteten.</span><span class="sxs-lookup"><span data-stu-id="0bc40-128">**Partner user**—the partner associated with the activity.</span></span>

5. <span data-ttu-id="0bc40-129">Välj **Exportera logg** för att kopiera kundens prenumerations data till en. csv-fil och ladda ned den till standardmappen för hämtning på din dator.</span><span class="sxs-lookup"><span data-stu-id="0bc40-129">Select **Export log** to copy the customer's subscription data into a .csv file and download it to the default download folder on your computer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0bc40-130">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="0bc40-130">Next steps</span></span>

- [<span data-ttu-id="0bc40-131">Analysera prenumerationer och licenser för att hjälpa till att driva affärs beslut</span><span class="sxs-lookup"><span data-stu-id="0bc40-131">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)
