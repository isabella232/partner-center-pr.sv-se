---
title: Partner Center Insights rollbaserad åtkomst
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig mer om de specifika roller som behövs för att se Partner Center Insights-rapporter. Dessa omfattar rollerna Executive Report Viewer och Report Viewer.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6af9c7d674d1956332a564628b6b2ea0b1796f6
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120791"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="8e4f3-104">Rollbaserad åtkomstkontroll till instrumentpanelen i Partnercenter Insights</span><span class="sxs-lookup"><span data-stu-id="8e4f3-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="8e4f3-105">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="8e4f3-105">**Appropriate roles**</span></span>

- <span data-ttu-id="8e4f3-106">Global administratör</span><span class="sxs-lookup"><span data-stu-id="8e4f3-106">Global admin</span></span>
- <span data-ttu-id="8e4f3-107">Administratörsagent</span><span class="sxs-lookup"><span data-stu-id="8e4f3-107">Admin agent</span></span>
- <span data-ttu-id="8e4f3-108">Rapportvisningsprogram</span><span class="sxs-lookup"><span data-stu-id="8e4f3-108">Report viewer</span></span>
- <span data-ttu-id="8e4f3-109">Visningsprogram för exekutiv rapport</span><span class="sxs-lookup"><span data-stu-id="8e4f3-109">Executive report viewer</span></span>

<span data-ttu-id="8e4f3-110">Insights-instrumentpanelen använder två nya roller i Partnercenter för att hantera medarbetares åtkomst till rapporterna – Visningsprogrammet för exekutiv rapport och rapportvisningsprogrammet.</span><span class="sxs-lookup"><span data-stu-id="8e4f3-110">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="8e4f3-111">Användare i rollen Visningsprogram för verkställande rapporter har åtkomst till alla rapportdatamängder, medan användare i rollen Rapportvisning inte har åtkomst till känsliga datauppsättningar, till exempel intäkter och kund-/medarbetares personliga data.</span><span class="sxs-lookup"><span data-stu-id="8e4f3-111">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="8e4f3-112">Precis som med andra Partnercenter-roller kommer den globala administratören eller kontoadministratören att kunna tilldela användare till dessa roller på sidan Användarhantering.</span><span class="sxs-lookup"><span data-stu-id="8e4f3-112">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="8e4f3-113">Rollerna kan tillämpas på hela företaget eller för specifika MPN-platser.</span><span class="sxs-lookup"><span data-stu-id="8e4f3-113">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="8e4f3-114">Roller som tilldelats för specifika MPN-platser begränsar användaren till att visa rapportdata som endast är associerade med de valda MPN-platserna.</span><span class="sxs-lookup"><span data-stu-id="8e4f3-114">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="8e4f3-115">Partner kan välja en eller flera platser i vyn nedan.</span><span class="sxs-lookup"><span data-stu-id="8e4f3-115">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Visar platsspecifika inställningar för Partner Center Insights-roller för rapportvisningsprogrammet och rapportvisningsprogrammet.":::

>[!Note]
> <span data-ttu-id="8e4f3-117">Användare som är MPN-administratörer från och med den 20 januari 2020 läggs automatiskt till i företagsomfattande **rollen Executive Report Viewer** för alla platser för den klientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="8e4f3-117">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="8e4f3-118">Dessa användare kan därför komma åt rapporterna som visningsprogram för exekutiv rapport utan uttryckliga åtgärder som krävs av global administratör eller kontoadministratör. Globala administratörer och kontoadministratörer kan åsidosätta de automatiskt tilldelade rollerna för dessa användare för att ytterligare öka eller begränsa deras funktioner.</span><span class="sxs-lookup"><span data-stu-id="8e4f3-118">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8e4f3-119">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="8e4f3-119">Next steps</span></span>

- <span data-ttu-id="8e4f3-120">Läs mer om [Partner Center Insights](partner-center-insights.md) och dess olika rapporter.</span><span class="sxs-lookup"><span data-stu-id="8e4f3-120">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
