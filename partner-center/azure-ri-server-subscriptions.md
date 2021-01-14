---
title: Azure-reservationer & Server prenumerationer
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig mer om moln lösnings leverantörens möjligheter att förvärva, etablera och hantera Azure-reservationer och Server prenumerationer för kunder.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d5386dd4b2b19e641cc9d731d4a3d0f44ab5ad6
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182502"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="93d65-103">Hämta, etablera & hantera reserverade VM-instanser (RI) + Server prenumerationer för kunder</span><span class="sxs-lookup"><span data-stu-id="93d65-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>


<span data-ttu-id="93d65-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="93d65-104">**Appropriate roles**</span></span>

- <span data-ttu-id="93d65-105">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="93d65-105">Admin agent</span></span>
- <span data-ttu-id="93d65-106">Global administratör</span><span class="sxs-lookup"><span data-stu-id="93d65-106">Global admin</span></span>
- <span data-ttu-id="93d65-107">Support agent</span><span class="sxs-lookup"><span data-stu-id="93d65-107">Helpdesk agent</span></span>
- <span data-ttu-id="93d65-108">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="93d65-108">Sales agent</span></span>
- <span data-ttu-id="93d65-109">Administratör för användar hantering</span><span class="sxs-lookup"><span data-stu-id="93d65-109">User management admin</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="93d65-110">Vad är Azure Reservations?</span><span class="sxs-lookup"><span data-stu-id="93d65-110">What are Azure Reservations?</span></span>

<span data-ttu-id="93d65-111">Azure Reservations hjälpa dig att spara pengar genom förskotts betalning för ett år eller tre års virtuell dator, SQL Database beräknings kapacitet, Azure Cosmos DB data flöde eller andra Azure-resurser.</span><span class="sxs-lookup"><span data-stu-id="93d65-111">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="93d65-112">Med förbetald betalning får du rabatt på de resurser du använder.</span><span class="sxs-lookup"><span data-stu-id="93d65-112">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="93d65-113">Reservationer kan avsevärt minska din virtuella dator, SQL Database Compute, Azure Cosmos DB och andra resurs kostnader upp till 72% jämfört med priset för betala per användning.</span><span class="sxs-lookup"><span data-stu-id="93d65-113">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="93d65-114">Reservation ger en rabatt och påverkar inte resursernas körningsstatus.</span><span class="sxs-lookup"><span data-stu-id="93d65-114">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="93d65-115">Mer information finns i [Vad är Azure reservations?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="93d65-115">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="93d65-116">Varför bör kunderna köpa en reservation?</span><span class="sxs-lookup"><span data-stu-id="93d65-116">Why should customers buy a reservation?</span></span>

<span data-ttu-id="93d65-117">Om kunder har virtuella datorer, Azure Cosmos DB eller SQL-databaser som körs under långa tids perioder, ger det mest kostnads effektiva alternativ att köpa en reservation.</span><span class="sxs-lookup"><span data-stu-id="93d65-117">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="93d65-118">Om till exempel en kund kontinuerligt kör fyra instanser av en tjänst utan en reservation debiteras de enligt priserna för betala per användning.</span><span class="sxs-lookup"><span data-stu-id="93d65-118">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="93d65-119">Om de köper en reservation för dessa resurser får de direkt reservations rabatten.</span><span class="sxs-lookup"><span data-stu-id="93d65-119">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="93d65-120">Resurserna debiteras inte längre enligt priserna för betala per användning.</span><span class="sxs-lookup"><span data-stu-id="93d65-120">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="93d65-121">Övertygande nytt Azure-erbjudande i CSP</span><span class="sxs-lookup"><span data-stu-id="93d65-121">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="93d65-122">Genom att ta Azure Reservations-och Server prenumerationer till sitt CSP-program, är Microsoft bättre för våra partner att ta itu med växande kund efter frågan för att få mer kostnads effektiva lösningar som stöd för förutsägbara, beständiga moln arbets belastningar.</span><span class="sxs-lookup"><span data-stu-id="93d65-122">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="93d65-123">CSP-programmet gör det möjligt för partner att förvärva, etablera och hantera Azure Reservations-och Server prenumerationer åt kommersiella kunder via Microsoft Partner Center och Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="93d65-123">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>
<span data-ttu-id="93d65-124">Vi ger även partner i våra CSP-program val om hur Azure-reservationer kan köpas.</span><span class="sxs-lookup"><span data-stu-id="93d65-124">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="93d65-125">CSP-partner kan [köpa Azure-reservationer för en kunds räkning](azure-reservations-buying.md) , eller så kan [kunden köpa sina egna reservationer](give-customers-permission.md) från en tidigare Azure-prenumeration som partnern har köpt för dem.</span><span class="sxs-lookup"><span data-stu-id="93d65-125">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="93d65-126">Azure Reservations ger kunderna flexibiliteten i virtualisering för en mängd olika data behandlings lösningar, inklusive utveckling och testning, körning av program och utökning av data centret.</span><span class="sxs-lookup"><span data-stu-id="93d65-126">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="93d65-127">Med [Azure Reserved VM instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) till exempel kan kommersiella kunder nu Spara upp till 72% jämfört med att betala per användning genom att köpa eller "reservera" – den virtuella datorn för en 1-eller tre års period.</span><span class="sxs-lookup"><span data-stu-id="93d65-127">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="93d65-128">Windows Server-kunder med Azure Hybrid-förmån, som ingår i Software Assurance, kan spara upp till 80% jämfört med priset enligt principen betala per användning.</span><span class="sxs-lookup"><span data-stu-id="93d65-128">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="93d65-129">Med en omatchad kombination av tvingande priser och oöverträffad distribution, ser kunderna det bästa generella värdet när de väljer Azure Reservations.</span><span class="sxs-lookup"><span data-stu-id="93d65-129">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations.</span></span>

- <span data-ttu-id="93d65-130">Se [inköps reservationer](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) på Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="93d65-130">See [Purchase Reservations](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) on the Azure Portal.</span></span>

- <span data-ttu-id="93d65-131">Se den **kommersiella pris listan för Azure RI-CSP** i kategorin **Microsoft Azure reserverade instanser** på sidan [priser och erbjudanden](https://partner.microsoft.com/dashboard/sell/pricingandoffers) i Partner Center för program varu prenumerationer och årliga prenumerationer för Linux ISV.</span><span class="sxs-lookup"><span data-stu-id="93d65-131">See the **Azure RI CSP Commercial Price List** under the **Microsoft Azure Reserved Instances** category on the [Pricing and Offers](https://partner.microsoft.com/dashboard/sell/pricingandoffers) page in Partner Center for software subscriptions and Linux ISV annual subscriptions.</span></span>


 
<span data-ttu-id="93d65-132">**Årliga prenumerationer för Linux ISV**</span><span class="sxs-lookup"><span data-stu-id="93d65-132">**Linux ISV annual subscriptions**</span></span>

- <span data-ttu-id="93d65-133">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="93d65-133">SUSE Linux</span></span>
- <span data-ttu-id="93d65-134">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="93d65-134">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="93d65-135">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="93d65-135">Azure Red Hat OpenShift</span></span>

<span data-ttu-id="93d65-136">**Årliga ISV-prenumerationer**</span><span class="sxs-lookup"><span data-stu-id="93d65-136">**ISV annual subscriptions**</span></span>

- <span data-ttu-id="93d65-137">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="93d65-137">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="93d65-138">Komma igång</span><span class="sxs-lookup"><span data-stu-id="93d65-138">Getting started</span></span>

<span data-ttu-id="93d65-139">För att förstå hur du kan placera Azure Reservations med dina kunder och komma igång så snabbt som möjligt rekommenderar vi följande tillvägagångs sätt för att granska beredskaps materialet:</span><span class="sxs-lookup"><span data-stu-id="93d65-139">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="93d65-140">Läs och förstå [partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span><span class="sxs-lookup"><span data-stu-id="93d65-140">Review and understand the [Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

2. <span data-ttu-id="93d65-141">Förstå uppdateringar för Azure Reservations-och Server prenumerationer i [partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances).</span><span class="sxs-lookup"><span data-stu-id="93d65-141">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances).</span></span>


### <a name="sales-readiness"></a><span data-ttu-id="93d65-142">Sälj beredskap</span><span class="sxs-lookup"><span data-stu-id="93d65-142">Sales readiness</span></span>

- [<span data-ttu-id="93d65-143">Fjärrskrivbordstjänster (RDS) klient åtkomst licens (CAL) (meddelande)</span><span class="sxs-lookup"><span data-stu-id="93d65-143">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [<span data-ttu-id="93d65-144">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="93d65-144">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [<span data-ttu-id="93d65-145">Server prenumerationer</span><span class="sxs-lookup"><span data-stu-id="93d65-145">Server Subscriptions</span></span>](./csp-software-subscriptions.md)

- [<span data-ttu-id="93d65-146">SQL DB-reservationer (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="93d65-146">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)

- [<span data-ttu-id="93d65-147">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="93d65-147">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)

- [<span data-ttu-id="93d65-148">SQL-hanterad instans (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="93d65-148">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)

- [<span data-ttu-id="93d65-149">SUSE och Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="93d65-149">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)

- [<span data-ttu-id="93d65-150">Red Hat Linux på Azure</span><span class="sxs-lookup"><span data-stu-id="93d65-150">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)

- [<span data-ttu-id="93d65-151">SUSE Linux på Azure</span><span class="sxs-lookup"><span data-stu-id="93d65-151">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [<span data-ttu-id="93d65-152">Linux på Azure</span><span class="sxs-lookup"><span data-stu-id="93d65-152">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)

- [<span data-ttu-id="93d65-153">Pris översikt för Azure</span><span class="sxs-lookup"><span data-stu-id="93d65-153">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)

- [<span data-ttu-id="93d65-154">Pris kalkylator för Azure</span><span class="sxs-lookup"><span data-stu-id="93d65-154">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)

- [<span data-ttu-id="93d65-155">Azure Databricks enhets reservationer</span><span class="sxs-lookup"><span data-stu-id="93d65-155">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a><span data-ttu-id="93d65-156">Utbildning</span><span class="sxs-lookup"><span data-stu-id="93d65-156">Training</span></span>

<span data-ttu-id="93d65-157">Registrera dig för att se [beredskap för webb seminarier](https://commercial-licensing.eventbuilder.com/FY2019_ALL) och händelser på begäran.</span><span class="sxs-lookup"><span data-stu-id="93d65-157">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>
<span data-ttu-id="93d65-158">Tidigare registrerade licens beredskap på begäran-händelser innehåller ämnen som:</span><span class="sxs-lookup"><span data-stu-id="93d65-158">Previously recorded Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="93d65-159">CSP online-tjänster, CSP Azure och allmänna licensierings uppdateringar, inklusive Azure (november 2018)</span><span class="sxs-lookup"><span data-stu-id="93d65-159">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>

- <span data-ttu-id="93d65-160">Flexibilitet för reserverad SQL DB-& instans storlek (augusti 2018)</span><span class="sxs-lookup"><span data-stu-id="93d65-160">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>

- <span data-ttu-id="93d65-161">Server prenumerationer i CSP (2018 juli)</span><span class="sxs-lookup"><span data-stu-id="93d65-161">Server Subscriptions in CSP (July 2018)</span></span>

- <span data-ttu-id="93d65-162">Azure Reservations översikt i CSP (maj 2018)</span><span class="sxs-lookup"><span data-stu-id="93d65-162">Azure Reservations Overview in CSP (May 2018)</span></span>

## <a name="operations"></a><span data-ttu-id="93d65-163">Operations</span><span class="sxs-lookup"><span data-stu-id="93d65-163">Operations</span></span>

<span data-ttu-id="93d65-164">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf): omfattande vägledning som täcker viktiga principer och drifts aspekter, till exempel avtal, beställning via partner Center, faktura, pris lista, incitament, avstämnings fil, API/SDK, Sandbox och Azure-partner delade tjänster.</span><span class="sxs-lookup"><span data-stu-id="93d65-164">[Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf):  Comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="93d65-165">Azure Hybrid-förmån</span><span class="sxs-lookup"><span data-stu-id="93d65-165">Azure Hybrid Benefit</span></span>

<span data-ttu-id="93d65-166">[Azure Hybrid-förmån](https://azure.microsoft.com/pricing/hybrid-benefit) är en pris förmån för kunder som har licenser med Software Assurance, vilket bidrar till att maximera värdet av befintliga lokala Windows Server-och/eller SQL Server licens investeringar vid migrering till Azure.</span><span class="sxs-lookup"><span data-stu-id="93d65-166">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is a pricing benefit for customers who have licenses with Software Assurance, which helps maximize the value of existing on-premises Windows Server and/or SQL Server license investments when migrating to Azure.</span></span> <span data-ttu-id="93d65-167">Berättigade kunder kan spara upp till 40% \* på Azure Virtual Machines (infrastruktur som en tjänst eller IaaS) och Spara upp till 55% på Azure SQL Database (plattform som en tjänst eller PaaS) och SQL Server på Azure Virtual Machines (IaaS) med Azure Hybrid-förmån, vilket ökar till upp till 80% i kombination med reserverade instanser i Azure.</span><span class="sxs-lookup"><span data-stu-id="93d65-167">Eligible customers can save up to 40%\* on Azure Virtual Machines (infrastructure as a service, or IaaS), and save up to 55% on Azure SQL Database (platform as a service, or PaaS) and SQL Server on Azure Virtual Machines (IaaS) with Azure Hybrid Benefit, which increases to up to 80% when combined with Azure Reserved Instances.</span></span>

## <a name="next-steps"></a><span data-ttu-id="93d65-168">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="93d65-168">Next steps</span></span>

- [<span data-ttu-id="93d65-169">Vanliga frågor och svar om Azure Hybrid-förmån</span><span class="sxs-lookup"><span data-stu-id="93d65-169">Azure Hybrid Benefit FAQ</span></span>](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

<span data-ttu-id="93d65-170">\* De faktiska besparingarna kan variera beroende på region, instans typ eller användning.</span><span class="sxs-lookup"><span data-stu-id="93d65-170">\*Actual savings may vary based on region, instance type, or usage.</span></span>