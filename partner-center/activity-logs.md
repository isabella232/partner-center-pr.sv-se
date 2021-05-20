---
title: Få insikter med kundaktivitetsloggar
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du visar och exporterar aktivitetsloggar för att få insikter om kundkontotransaktioner och andra kundrelaterade partnerhanteringsaktiviteter.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1bb98dd71c9e46914b90d5efbfe14404d08275f9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150598"
---
# <a name="view-or-export-customer-activity-logs-for-more-insight-into-customer-transactions"></a><span data-ttu-id="ae80c-103">Visa eller exportera kundaktivitetsloggar för mer information om kundtransaktioner</span><span class="sxs-lookup"><span data-stu-id="ae80c-103">View or export customer activity logs for more insight into customer transactions</span></span>

<span data-ttu-id="ae80c-104">**Lämpliga roller:** Globala | Faktureringsadministratörskonto | Administratörsbehörighet för | Administratörsagent | Försäljningsagent | Supportagent</span><span class="sxs-lookup"><span data-stu-id="ae80c-104">**Appropriate roles**: Global admin | Billing admin | User management admin | Admin agent | Sales agent | Helpdesk agent</span></span>

<span data-ttu-id="ae80c-105">Aktivitetsloggar ger information om transaktioner och partnerhanteringsåtgärder för kunder.</span><span class="sxs-lookup"><span data-stu-id="ae80c-105">Activity logs provide information on transactions and Partner management actions for customers.</span></span> <span data-ttu-id="ae80c-106">Loggar för transaktioner innehåller detaljerad information om transaktionen, inklusive köpta prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="ae80c-106">Logs for transactions provide detailed information about the transaction, including purchased subscriptions.</span></span> <span data-ttu-id="ae80c-107">Du kan också exportera aktivitetsloggar till ett Excel-kompatibelt filformat med kommaavgränsade värden (.csv).</span><span class="sxs-lookup"><span data-stu-id="ae80c-107">You can also export activity logs to an Excel-compatible comma-separated value file format (.csv).</span></span>

<span data-ttu-id="ae80c-108">Aktivitetsloggar innehåller poster för partneråtgärder för kundkonton och produkttransaktioner.</span><span class="sxs-lookup"><span data-stu-id="ae80c-108">Activity logs provide records for Partner actions on customer accounts and product transactions.</span></span> <span data-ttu-id="ae80c-109">Du kan också exportera aktivitetsloggar till en CSV-fil.</span><span class="sxs-lookup"><span data-stu-id="ae80c-109">You can also export activity logs to a .csv file.</span></span>

## <a name="view-and-export-activity-logs"></a><span data-ttu-id="ae80c-110">Visa och exportera aktivitetsloggar</span><span class="sxs-lookup"><span data-stu-id="ae80c-110">View and export activity logs</span></span>

1. <span data-ttu-id="ae80c-111">Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="ae80c-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="ae80c-112">På menyn **Kontoinställningar** väljer du **Aktivitetslogg.**</span><span class="sxs-lookup"><span data-stu-id="ae80c-112">From the **Account settings** menu, select **Activity Log**.</span></span>

3. <span data-ttu-id="ae80c-113">Välj aktivitetsloggperiod i fälten **Från** **och till.**</span><span class="sxs-lookup"><span data-stu-id="ae80c-113">Select the activity log period in the **From** and **to** fields.</span></span> <span data-ttu-id="ae80c-114">Aktivitetsloggexporten är som standard den senaste månaden.</span><span class="sxs-lookup"><span data-stu-id="ae80c-114">The activity log export defaults to the most recent month.</span></span>

   <span data-ttu-id="ae80c-115">Varje aktivitetslogg innehåller en länk till kundens **prenumerationssida i** listan.</span><span class="sxs-lookup"><span data-stu-id="ae80c-115">Each activity log provides a link to the listed customer's **Subscriptions** page.</span></span>

   <span data-ttu-id="ae80c-116">Välj en nedåtpil för en aktivitetslogg om du vill visa information om en loggad åtgärd.</span><span class="sxs-lookup"><span data-stu-id="ae80c-116">Select a down arrow for any activity log to view details about a logged action.</span></span> <span data-ttu-id="ae80c-117">En enda aktivitetslogg kan visa en stor mängd data, till exempel beställning av flera produkter.</span><span class="sxs-lookup"><span data-stu-id="ae80c-117">A single activity log can show a significant amount of data, such as the ordering of multiple products.</span></span>

4. <span data-ttu-id="ae80c-118">Loggens datakolumner omfattar följande:</span><span class="sxs-lookup"><span data-stu-id="ae80c-118">The data columns of the log include the following:</span></span>
   - <span data-ttu-id="ae80c-119">**Date-Time**– datum och tid för åtgärden;</span><span class="sxs-lookup"><span data-stu-id="ae80c-119">**Date-Time**-the date and time of the action;</span></span>
   - <span data-ttu-id="ae80c-120">**Berörd** kund – kundens företagsnamn;</span><span class="sxs-lookup"><span data-stu-id="ae80c-120">**Affected customer**—the customer's company name;</span></span>
   - <span data-ttu-id="ae80c-121">**Åtgärd**– den åtgärd som vidtas av kunden, till exempel "skapad en hänvisning";</span><span class="sxs-lookup"><span data-stu-id="ae80c-121">**Action**—the action taken by the customer such as "created a referral";</span></span>
   - <span data-ttu-id="ae80c-122">**Partneranvändare**– partnern som är associerad med aktiviteten.</span><span class="sxs-lookup"><span data-stu-id="ae80c-122">**Partner user**—the partner associated with the activity.</span></span>

5. <span data-ttu-id="ae80c-123">Välj **Exportera logg** för att kopiera kundens prenumerationsdata till en CSV-fil och ladda ned dem till standardnedladdningsmappen på datorn.</span><span class="sxs-lookup"><span data-stu-id="ae80c-123">Select **Export log** to copy the customer's subscription data into a .csv file and download it to the default download folder on your computer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ae80c-124">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ae80c-124">Next steps</span></span>

- [<span data-ttu-id="ae80c-125">Analysera prenumerationer och licenser för att fatta affärsbeslut</span><span class="sxs-lookup"><span data-stu-id="ae80c-125">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)
