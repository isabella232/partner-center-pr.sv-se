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
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a>Hämta, etablera & hantera reserverade VM-instanser (RI) + Server prenumerationer för kunder

Gäller för:

- Partnercenter

**Lämpliga roller**

- Administratörs agent
- Global administratör
- Support agent
- Försäljnings agent
- Administratör för användar hantering

> [!NOTE]
> Den här artikeln gäller endast partner i Cloud Solution Provider (CSP)-programmet. Kunder som använder andra typer av prenumerationer (t. ex. betala per användning, enskilda, Microsoft-kundavtal eller Enterprise-avtal prenumerationer) bör i stället läsa [denna dokumentation om Azure-reservationer](/azure/cost-management-billing/reservations).


## <a name="what-are-azure-reservations"></a>Vad är Azure Reservations?

Azure Reservations hjälpa dig att spara pengar genom förskotts betalning för ett år eller tre års virtuell dator, SQL Database beräknings kapacitet, Azure Cosmos DB data flöde eller andra Azure-resurser. Med förbetald betalning får du rabatt på de resurser du använder. Reservationer kan avsevärt minska din virtuella dator, SQL Database Compute, Azure Cosmos DB och andra resurs kostnader upp till 72% jämfört med priset för betala per användning. Reservation ger en rabatt och påverkar inte resursernas körningsstatus. Mer information finns i [Vad är Azure reservations?](/azure/billing/billing-save-compute-costs-reservations)

## <a name="why-should-customers-buy-a-reservation"></a>Varför bör kunderna köpa en reservation?

Om kunder har virtuella datorer, Azure Cosmos DB eller SQL-databaser som körs under långa tids perioder, ger det mest kostnads effektiva alternativ att köpa en reservation. Om till exempel en kund kontinuerligt kör fyra instanser av en tjänst utan en reservation debiteras de enligt priserna för betala per användning. Om de köper en reservation för dessa resurser får de direkt reservations rabatten. Resurserna debiteras inte längre enligt priserna för betala per användning.

### <a name="compelling-new-azure-offer-in-csp"></a>Övertygande nytt Azure-erbjudande i CSP

Genom att ta Azure Reservations-och Server prenumerationer till sitt CSP-program, är Microsoft bättre för våra partner att ta itu med växande kund efter frågan för att få mer kostnads effektiva lösningar som stöd för förutsägbara, beständiga moln arbets belastningar. CSP-programmet gör det möjligt för partner att förvärva, etablera och hantera Azure Reservations-och Server prenumerationer åt kommersiella kunder via Microsoft Partner Center och Azure Portal.

Vi ger även partner i våra CSP-program val om hur Azure-reservationer kan köpas. CSP-partner kan [köpa Azure-reservationer för en kunds räkning](azure-reservations-buying.md) , eller så kan [kunden köpa sina egna reservationer](give-customers-permission.md) från en tidigare Azure-prenumeration som partnern har köpt för dem.

Azure Reservations ger kunderna flexibiliteten i virtualisering för en mängd olika data behandlings lösningar, inklusive utveckling och testning, körning av program och utökning av data centret.

Med [Azure Reserved VM instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) till exempel kan kommersiella kunder nu Spara upp till 72% jämfört med att betala per användning genom att köpa eller "reservera" – den virtuella datorn för en 1-eller tre års period. Windows Server-kunder med Azure Hybrid-förmån, som ingår i Software Assurance, kan spara upp till 80% jämfört med priset enligt principen betala per användning.

Med en omatchad kombination av tvingande priser och oöverträffad distribution, ser kunderna det bästa generella värdet när de väljer Azure Reservations:

#### <a name="azure-reservations"></a>Azure-reservationer

- Azure Reserved VM Instances
- SQL DB-reservationer
- SQL-hanterad instans
- Azure Cosmos DB
- Azure SQL Data Warehouse
- App Services
- Azure Databricks enhets reservationer
- Hanterad disk
- Blockblob
- MySQL
- Azure Data Explorer
- MariaDB
- PostgreSQL

#### <a name="server-subscriptions"></a>Server prenumerationer

- Windows Server
- Klient åtkomst licenser för Fjärrskrivbordstjänster (RDS)
- SQL Server

#### <a name="linux-isv-annual-subscriptions"></a>Årliga prenumerationer för Linux ISV

- SUSE Linux
- Red Hat Enterprise Linux
- Azure Red Hat OpenShift

#### <a name="isv-annual-subscriptions"></a>Årliga ISV-prenumerationer

- Azure VMware Solution by CloudSimple

## <a name="getting-started"></a>Komma igång

För att förstå hur du kan placera Azure Reservations med dina kunder och komma igång så snabbt som möjligt rekommenderar vi följande tillvägagångs sätt för att granska beredskaps materialet:

1. Granska översikts presentationerna och tillhör ande webb seminarier för kund värdens förslag och placering
2. Läs och förstå den moderna handels guiden för Commerce
3. Läs vanliga frågor och svar om Azure RI och Server prenumerationer
4. Förstå uppdateringar för Azure Reservations-och Server prenumerationer i [partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)

## <a name="resources"></a>Resurser

Nedan finns en omfattande lista över resurser som hjälper dig att snabbt kunna interagera Azure Reservations via partner Center:

### <a name="sales-readiness"></a>Sälj beredskap

- [Azure Reservations-och Server prenumerationer med Azure Hybrid-förmån översikt](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [Försäljnings blad](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [Vanliga frågor och svar om partner för Azure Reservations](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [Vanliga frågor och svar om partner för Azure Reservations och SQL DB](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [Fjärrskrivbordstjänster (RDS) klient åtkomst licens (CAL) (meddelande)](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [Azure Reserved VM Instances (Azure Portal)](/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [Server prenumerationer](csp-software-subscriptions.md)
- [Översikt över SQL DB i Azure](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [SQL DB-reservationer (Azure Portal)](/azure/sql-database/sql-database-reserved-capacity)
- [Azure Cosmos DB (Azure Portal)](/azure/cosmos-db/cosmos-db-reserved-capacity)
- [SQL-hanterad instans (Azure Portal)](/azure/sql-database/sql-database-managed-instance)
- [SUSE och Red Hat Enterprise Linux (Azure Portal)](/azure/virtual-machines/linux/prepay-suse-software-charges)
- [Red Hat Linux på Azure](https://azure.com/redhat)
- [SUSE Linux på Azure](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [Linux på Azure](https://azure.microsoft.com/overview/linux-on-azure/)
- [Pris översikt för Azure](https://azure.microsoft.com/pricing/)
- [Pris kalkylator för Azure](https://azure.microsoft.com/pricing/calculator)
- [Azure Databricks enhets reservationer](/azure/billing/billing-prepay-databricks-reserved-capacity)
- CSP-pris listor: pris listorna **Microsoft Azure reserverade instanser** och **program varu prenumerationer** finns både på sidan med pris information för Partner Center på [pris &](https://partner.microsoft.com/pcv/sales) .

### <a name="training"></a>Utbildning

Registrera dig för att se [beredskap för webb seminarier](https://commercial-licensing.eventbuilder.com/FY2019_ALL) och händelser på begäran.

Licensierings beredskap på begäran-händelser innehåller ämnen som:

- CSP online-tjänster, CSP Azure och allmänna licensierings uppdateringar, inklusive Azure (november 2018)
- Flexibilitet för reserverad SQL DB-& instans storlek (augusti 2018)
- Server prenumerationer i CSP (2018 juli)
- Azure Reservations översikt i CSP (maj 2018)

Annan användbar utbildning omfattar [Azure-klientlicensieringstjänsten på partner University](https://aka.ms/azure_partner_licensing).

### <a name="operations"></a>Åtgärder

- [Hand bok för hand boken](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (uppdaterad): en omfattande guide som täcker viktiga principer och drifts aspekter, till exempel avtal, beställning via partner Center, faktura, pris lista, incitament, avstämnings fil, API/SDK, Sandbox och Azure-partner delade tjänster.
- [Modern erbjuder lands tillgänglighet och kund valuta mat ris](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [Sälj Microsoft Azure reserverade instanser](azure-reservations.md)
- [Köp Microsoft Azure reservationer för kundernas räkning](azure-reservations-buying.md)
- [Hantera Azure-reservationer för kundernas räkning](azure-reservations-manage.md)
- [Fakturering för Azure-reservationer](azure-plan-billing.md)
- [Storlek på virtuell dator för maximal reservations användning](azure-usage.md)
- [API för partner Center (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)
- [Fjärrskrivbordstjänster](/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a>Azure Hybrid-förmån

[Azure Hybrid-förmån](https://azure.microsoft.com/pricing/hybrid-benefit) hjälper dig att få mer värde från dina Windows Server-licenser och Spara upp till * 47 procent på virtuella datorer. Du kan använda fördelarna med Windows Server Data Center och Standard Edition-licenser som omfattas av Software Assurance. Beroende på versionen kan du konvertera eller återanvända dina licenser för att köra virtuella Windows Server-datorer i Azure och betala en lägre bas beräknings pris (priser för virtuella Linux-datorer).

Se även [Azure Hybrid-förmån vanliga frågor och svar](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

* De faktiska besparingarna kan variera beroende på region, instans typ eller användning.
