---
title: Azure-reservationer & Server prenumerationer
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig mer om moln lösnings leverantörens möjligheter att förvärva, etablera och hantera Azure-reservationer och Server prenumerationer för kunder.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3c08e897a8f5d7c11b36627b0c24ad2da3f92329
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531625"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="aa488-103">Hämta, etablera & hantera reserverade VM-instanser (RI) + Server prenumerationer för kunder</span><span class="sxs-lookup"><span data-stu-id="aa488-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="aa488-104">Gäller för:</span><span class="sxs-lookup"><span data-stu-id="aa488-104">Applies to:</span></span>

- <span data-ttu-id="aa488-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="aa488-105">Partner Center</span></span>

<span data-ttu-id="aa488-106">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="aa488-106">**Appropriate roles**</span></span>

- <span data-ttu-id="aa488-107">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="aa488-107">Admin agent</span></span>
- <span data-ttu-id="aa488-108">Global administratör</span><span class="sxs-lookup"><span data-stu-id="aa488-108">Global admin</span></span>
- <span data-ttu-id="aa488-109">Support agent</span><span class="sxs-lookup"><span data-stu-id="aa488-109">Helpdesk agent</span></span>
- <span data-ttu-id="aa488-110">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="aa488-110">Sales agent</span></span>
- <span data-ttu-id="aa488-111">Administratör för användar hantering</span><span class="sxs-lookup"><span data-stu-id="aa488-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="aa488-112">Den här artikeln gäller endast partner i Cloud Solution Provider (CSP)-programmet.</span><span class="sxs-lookup"><span data-stu-id="aa488-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="aa488-113">Kunder som använder andra typer av prenumerationer (t. ex. betala per användning, enskilda, Microsoft-kundavtal eller Enterprise-avtal prenumerationer) bör i stället läsa [denna dokumentation om Azure-reservationer](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="aa488-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="aa488-114">Vad är Azure Reservations?</span><span class="sxs-lookup"><span data-stu-id="aa488-114">What are Azure Reservations?</span></span>

<span data-ttu-id="aa488-115">Azure Reservations hjälpa dig att spara pengar genom förskotts betalning för ett år eller tre års virtuell dator, SQL Database beräknings kapacitet, Azure Cosmos DB data flöde eller andra Azure-resurser.</span><span class="sxs-lookup"><span data-stu-id="aa488-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="aa488-116">Med förbetald betalning får du rabatt på de resurser du använder.</span><span class="sxs-lookup"><span data-stu-id="aa488-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="aa488-117">Reservationer kan avsevärt minska din virtuella dator, SQL Database Compute, Azure Cosmos DB och andra resurs kostnader upp till 72% jämfört med priset för betala per användning.</span><span class="sxs-lookup"><span data-stu-id="aa488-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="aa488-118">Reservation ger en rabatt och påverkar inte resursernas körningsstatus.</span><span class="sxs-lookup"><span data-stu-id="aa488-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="aa488-119">Mer information finns i [Vad är Azure reservations?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="aa488-119">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="aa488-120">Varför bör kunderna köpa en reservation?</span><span class="sxs-lookup"><span data-stu-id="aa488-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="aa488-121">Om kunder har virtuella datorer, Azure Cosmos DB eller SQL-databaser som körs under långa tids perioder, ger det mest kostnads effektiva alternativ att köpa en reservation.</span><span class="sxs-lookup"><span data-stu-id="aa488-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="aa488-122">Om till exempel en kund kontinuerligt kör fyra instanser av en tjänst utan en reservation debiteras de enligt priserna för betala per användning.</span><span class="sxs-lookup"><span data-stu-id="aa488-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="aa488-123">Om de köper en reservation för dessa resurser får de direkt reservations rabatten.</span><span class="sxs-lookup"><span data-stu-id="aa488-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="aa488-124">Resurserna debiteras inte längre enligt priserna för betala per användning.</span><span class="sxs-lookup"><span data-stu-id="aa488-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="aa488-125">Övertygande nytt Azure-erbjudande i CSP</span><span class="sxs-lookup"><span data-stu-id="aa488-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="aa488-126">Genom att ta Azure Reservations-och Server prenumerationer till sitt CSP-program, är Microsoft bättre för våra partner att ta itu med växande kund efter frågan för att få mer kostnads effektiva lösningar som stöd för förutsägbara, beständiga moln arbets belastningar.</span><span class="sxs-lookup"><span data-stu-id="aa488-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="aa488-127">CSP-programmet gör det möjligt för partner att förvärva, etablera och hantera Azure Reservations-och Server prenumerationer åt kommersiella kunder via Microsoft Partner Center och Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="aa488-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="aa488-128">Vi ger även partner i våra CSP-program val om hur Azure-reservationer kan köpas.</span><span class="sxs-lookup"><span data-stu-id="aa488-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="aa488-129">CSP-partner kan [köpa Azure-reservationer för en kunds räkning](azure-reservations-buying.md) , eller så kan [kunden köpa sina egna reservationer](give-customers-permission.md) från en tidigare Azure-prenumeration som partnern har köpt för dem.</span><span class="sxs-lookup"><span data-stu-id="aa488-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="aa488-130">Azure Reservations ger kunderna flexibiliteten i virtualisering för en mängd olika data behandlings lösningar, inklusive utveckling och testning, körning av program och utökning av data centret.</span><span class="sxs-lookup"><span data-stu-id="aa488-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="aa488-131">Med [Azure Reserved VM instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) till exempel kan kommersiella kunder nu Spara upp till 72% jämfört med att betala per användning genom att köpa eller "reservera" – den virtuella datorn för en 1-eller tre års period.</span><span class="sxs-lookup"><span data-stu-id="aa488-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="aa488-132">Windows Server-kunder med Azure Hybrid-förmån, som ingår i Software Assurance, kan spara upp till 80% jämfört med priset enligt principen betala per användning.</span><span class="sxs-lookup"><span data-stu-id="aa488-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="aa488-133">Med en omatchad kombination av tvingande priser och oöverträffad distribution, ser kunderna det bästa generella värdet när de väljer Azure Reservations:</span><span class="sxs-lookup"><span data-stu-id="aa488-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="aa488-134">Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="aa488-134">Azure reservations</span></span>

- <span data-ttu-id="aa488-135">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="aa488-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="aa488-136">SQL DB-reservationer</span><span class="sxs-lookup"><span data-stu-id="aa488-136">SQL DB Reservations</span></span>
- <span data-ttu-id="aa488-137">SQL-hanterad instans</span><span class="sxs-lookup"><span data-stu-id="aa488-137">SQL Managed Instance</span></span>
- <span data-ttu-id="aa488-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aa488-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="aa488-139">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="aa488-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="aa488-140">App Services</span><span class="sxs-lookup"><span data-stu-id="aa488-140">App Services</span></span>
- <span data-ttu-id="aa488-141">Azure Databricks enhets reservationer</span><span class="sxs-lookup"><span data-stu-id="aa488-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="aa488-142">Hanterad disk</span><span class="sxs-lookup"><span data-stu-id="aa488-142">Managed Disk</span></span>
- <span data-ttu-id="aa488-143">Blockblob</span><span class="sxs-lookup"><span data-stu-id="aa488-143">Block blob</span></span>
- <span data-ttu-id="aa488-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="aa488-144">MySQL</span></span>
- <span data-ttu-id="aa488-145">Azure Data Explorer</span><span class="sxs-lookup"><span data-stu-id="aa488-145">Azure Data explorer</span></span>
- <span data-ttu-id="aa488-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="aa488-146">MariaDB</span></span>
- <span data-ttu-id="aa488-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="aa488-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="aa488-148">Server prenumerationer</span><span class="sxs-lookup"><span data-stu-id="aa488-148">Server subscriptions</span></span>

- <span data-ttu-id="aa488-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="aa488-149">Windows Server</span></span>
- <span data-ttu-id="aa488-150">Klient åtkomst licenser för Fjärrskrivbordstjänster (RDS)</span><span class="sxs-lookup"><span data-stu-id="aa488-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="aa488-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="aa488-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="aa488-152">Årliga prenumerationer för Linux ISV</span><span class="sxs-lookup"><span data-stu-id="aa488-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="aa488-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="aa488-153">SUSE Linux</span></span>
- <span data-ttu-id="aa488-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="aa488-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="aa488-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="aa488-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="aa488-156">Årliga ISV-prenumerationer</span><span class="sxs-lookup"><span data-stu-id="aa488-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="aa488-157">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="aa488-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="aa488-158">Komma igång</span><span class="sxs-lookup"><span data-stu-id="aa488-158">Getting started</span></span>

<span data-ttu-id="aa488-159">För att förstå hur du kan placera Azure Reservations med dina kunder och komma igång så snabbt som möjligt rekommenderar vi följande tillvägagångs sätt för att granska beredskaps materialet:</span><span class="sxs-lookup"><span data-stu-id="aa488-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="aa488-160">Granska översikts presentationerna och tillhör ande webb seminarier för kund värdens förslag och placering</span><span class="sxs-lookup"><span data-stu-id="aa488-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="aa488-161">Läs och förstå den moderna handels guiden för Commerce</span><span class="sxs-lookup"><span data-stu-id="aa488-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="aa488-162">Läs vanliga frågor och svar om Azure RI och Server prenumerationer</span><span class="sxs-lookup"><span data-stu-id="aa488-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="aa488-163">Förstå uppdateringar för Azure Reservations-och Server prenumerationer i [partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="aa488-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="aa488-164">Resurser</span><span class="sxs-lookup"><span data-stu-id="aa488-164">Resources</span></span>

<span data-ttu-id="aa488-165">Nedan finns en omfattande lista över resurser som hjälper dig att snabbt kunna interagera Azure Reservations via partner Center:</span><span class="sxs-lookup"><span data-stu-id="aa488-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="aa488-166">Sälj beredskap</span><span class="sxs-lookup"><span data-stu-id="aa488-166">Sales readiness</span></span>

- [<span data-ttu-id="aa488-167">Azure Reservations-och Server prenumerationer med Azure Hybrid-förmån översikt</span><span class="sxs-lookup"><span data-stu-id="aa488-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="aa488-168">Försäljnings blad</span><span class="sxs-lookup"><span data-stu-id="aa488-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="aa488-169">Vanliga frågor och svar om partner för Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="aa488-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="aa488-170">Vanliga frågor och svar om partner för Azure Reservations och SQL DB</span><span class="sxs-lookup"><span data-stu-id="aa488-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="aa488-171">Fjärrskrivbordstjänster (RDS) klient åtkomst licens (CAL) (meddelande)</span><span class="sxs-lookup"><span data-stu-id="aa488-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="aa488-172">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="aa488-172">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="aa488-173">Server prenumerationer</span><span class="sxs-lookup"><span data-stu-id="aa488-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="aa488-174">Översikt över SQL DB i Azure</span><span class="sxs-lookup"><span data-stu-id="aa488-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="aa488-175">SQL DB-reservationer (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="aa488-175">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="aa488-176">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="aa488-176">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="aa488-177">SQL-hanterad instans (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="aa488-177">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="aa488-178">SUSE och Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="aa488-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="aa488-179">Red Hat Linux på Azure</span><span class="sxs-lookup"><span data-stu-id="aa488-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="aa488-180">SUSE Linux på Azure</span><span class="sxs-lookup"><span data-stu-id="aa488-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="aa488-181">Linux på Azure</span><span class="sxs-lookup"><span data-stu-id="aa488-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="aa488-182">Pris översikt för Azure</span><span class="sxs-lookup"><span data-stu-id="aa488-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="aa488-183">Pris kalkylator för Azure</span><span class="sxs-lookup"><span data-stu-id="aa488-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="aa488-184">Azure Databricks enhets reservationer</span><span class="sxs-lookup"><span data-stu-id="aa488-184">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="aa488-185">CSP-pris listor: pris listorna **Microsoft Azure reserverade instanser** och **program varu prenumerationer** finns både på sidan med pris information för Partner Center på [pris &](https://partner.microsoft.com/pcv/sales) .</span><span class="sxs-lookup"><span data-stu-id="aa488-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="aa488-186">Utbildning</span><span class="sxs-lookup"><span data-stu-id="aa488-186">Training</span></span>

<span data-ttu-id="aa488-187">Registrera dig för att se [beredskap för webb seminarier](https://commercial-licensing.eventbuilder.com/FY2019_ALL) och händelser på begäran.</span><span class="sxs-lookup"><span data-stu-id="aa488-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="aa488-188">Licensierings beredskap på begäran-händelser innehåller ämnen som:</span><span class="sxs-lookup"><span data-stu-id="aa488-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="aa488-189">CSP online-tjänster, CSP Azure och allmänna licensierings uppdateringar, inklusive Azure (november 2018)</span><span class="sxs-lookup"><span data-stu-id="aa488-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="aa488-190">Flexibilitet för reserverad SQL DB-& instans storlek (augusti 2018)</span><span class="sxs-lookup"><span data-stu-id="aa488-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="aa488-191">Server prenumerationer i CSP (2018 juli)</span><span class="sxs-lookup"><span data-stu-id="aa488-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="aa488-192">Azure Reservations översikt i CSP (maj 2018)</span><span class="sxs-lookup"><span data-stu-id="aa488-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="aa488-193">Annan användbar utbildning omfattar [Azure-klientlicensieringstjänsten på partner University](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="aa488-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="aa488-194">Åtgärder</span><span class="sxs-lookup"><span data-stu-id="aa488-194">Operations</span></span>

- <span data-ttu-id="aa488-195">[Hand bok för hand boken](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (uppdaterad): en omfattande guide som täcker viktiga principer och drifts aspekter, till exempel avtal, beställning via partner Center, faktura, pris lista, incitament, avstämnings fil, API/SDK, Sandbox och Azure-partner delade tjänster.</span><span class="sxs-lookup"><span data-stu-id="aa488-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="aa488-196">Modern erbjuder lands tillgänglighet och kund valuta mat ris</span><span class="sxs-lookup"><span data-stu-id="aa488-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="aa488-197">Sälj Microsoft Azure reserverade instanser</span><span class="sxs-lookup"><span data-stu-id="aa488-197">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md)
- [<span data-ttu-id="aa488-198">Köp Microsoft Azure reservationer för kundernas räkning</span><span class="sxs-lookup"><span data-stu-id="aa488-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)
- [<span data-ttu-id="aa488-199">Hantera Azure-reservationer för kundernas räkning</span><span class="sxs-lookup"><span data-stu-id="aa488-199">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)
- [<span data-ttu-id="aa488-200">Fakturering för Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="aa488-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="aa488-201">Storlek på virtuell dator för maximal reservations användning</span><span class="sxs-lookup"><span data-stu-id="aa488-201">VM sizing for maximum reservation usage</span></span>](azure-usage.md)
- [<span data-ttu-id="aa488-202">API för partner Center (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="aa488-202">Partner Center API (API/SDK)</span></span>](/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="aa488-203">Fjärrskrivbordstjänster</span><span class="sxs-lookup"><span data-stu-id="aa488-203">Remote Desktop Services</span></span>](/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="aa488-204">Azure Hybrid-förmån</span><span class="sxs-lookup"><span data-stu-id="aa488-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="aa488-205">[Azure Hybrid-förmån](https://azure.microsoft.com/pricing/hybrid-benefit) hjälper dig att få mer värde från dina Windows Server-licenser och Spara upp till \* 47 procent på virtuella datorer.</span><span class="sxs-lookup"><span data-stu-id="aa488-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="aa488-206">Du kan använda fördelarna med Windows Server Data Center och Standard Edition-licenser som omfattas av Software Assurance.</span><span class="sxs-lookup"><span data-stu-id="aa488-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="aa488-207">Beroende på versionen kan du konvertera eller återanvända dina licenser för att köra virtuella Windows Server-datorer i Azure och betala en lägre bas beräknings pris (priser för virtuella Linux-datorer).</span><span class="sxs-lookup"><span data-stu-id="aa488-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="aa488-208">Se även [Azure Hybrid-förmån vanliga frågor och svar](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="aa488-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="aa488-209">\* De faktiska besparingarna kan variera beroende på region, instans typ eller användning.</span><span class="sxs-lookup"><span data-stu-id="aa488-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
