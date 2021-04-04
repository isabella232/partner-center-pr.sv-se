---
title: Insikter för partner Center
description: 'Utforska den här instrument panelen för enhetlig rapportering i Partner Center. Se hur du arbetar i KPI: er för försäljning och distribution, kund utveckling och mycket mer.'
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: ba8389ff613b47b17b87a6769674e33948fdc37d
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086591"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a>Partner Center Insights – en instrument panel som visar hur en Microsoft-kommersiell partner gör

**Lämpliga roller**

- Global administratör
- Kontoadministratör
- Rapport visnings program för chefer
- Rapport visnings program

## <a name="introduction"></a>Introduktion

Insikts instrument panelen är en enhetlig rapport instrument panel i Partner Center för Microsofts kommersiella partner som har registrerats i Microsoft Partner Network-programmet (MPN). På instrument panelen insikter 360 får du en översikt över dina KPI: er (nyckeltal) över moln produkter som Office, Azure, Dynamics och licensierings modeller som CSP och EA. Den visar en omfattande uppsättning KPI-rapporter som kan hjälpa dig att fatta data drivna beslut för din organisation. 

## <a name="role-based-access-control-to-the-insights-dashboard"></a>Rollbaserad åtkomst kontroll på insiktens instrument panel

Det finns två nya roller i Partner Center utformade särskilt för att få till gång till insikter: **Report Viewer** och **Executive Report Viewer**. Användare i rollen Executive Report Viewer har åtkomst till alla rapport data uppsättningar, medan användare i Report Viewer-rollen inte har åtkomst till känsliga data uppsättningar, till exempel intäkter och kund/anställdas personliga data. 

Den globala administratören eller konto administratören kan tilldela användare roller och tilldelas antingen för hela företaget eller för en speciell MPN-plats.  

>[!Note] 
>Användare som var MPN administratörer från och med den 20 januari 2020 lades automatiskt till i rollen för rapport visnings programmet i hela företaget. De kan komma åt rapporterna som ett rapport visnings program utan uttryckliga åtgärder som krävs av global administratör eller konto administratör. De globala administratörerna eller konto administratören kan åsidosätta tilldelningarna om det behövs. 

## <a name="reports-available"></a>Tillgängliga rapporter

Följande rapporter är tillgängliga som en del av instrument panelen för insikter.

**Översikt**: översikts rapporten visar en Snapshot-vy över olika KPI: er som är intressanta för dig, till exempel kund antal, antal aktiva prenumerationer, Azure förbruknings intäkter, aktiva licenser osv.

**Kund**: kund rapporten visar analyser runt dina kunder, till exempel kund förvärvs data, aktiva kunder osv.

**Produkt prenumerationer**: prenumerations rapporten visar förvärvs-och användnings analyser för dina moln prenumerationer (till exempel O365, Azure, Dynamics osv.)

**Produkt licenser**: instrument panelen för licenser visar licens analys för licensbaserade moln produkter som O365, Dynamics, Power BI osv.

**Produkt – Azure-användning**: Azure-användnings rapporten visar statistik relaterade till dina kunders Azure-prenumerationer, inklusive Azures förbruknings intäkter och användning efter mätnings kategorier.

**Kompetenser**: rapporten kompetenser visar mått för din aktiva, kvalificerade och risk kompetens.

**Fördelar**: förmåns rapporten innehåller analyser av partner förmåner som du har intjänat kontra förbrukat.

## <a name="navigating-the-insights-reports"></a>Navigera i insikts rapporterna

**Datum intervall filter**: du kan hitta ett datum intervall i det övre högra hörnet på varje sida. Utdata från översikts sidans diagram kan anpassas genom att välja ett datum intervall baserat på de senaste 3, 6 eller 12 månaderna, eller genom att välja ett anpassat datum intervall. Standard valet för datum intervall är 12 månader. 

:::image type="content" source="images/pci/intro1.png" alt-text="Introduktions karta":::

**Knappen feedback**: varje diagram/kontroll i alla insikter-rapporter införlivas med en feedback-knapp så att du kan ge dig feedback om en rapport funktion. 

 
**Sid nivå filter**: förutom för översikts-, förmåns-och kompetens rapporter kan du använda filter på sidnivå för alla insikter-rapporter. 

- De filter som väljs gäller för alla diagram och mått på en sida, inklusive sammanfattnings avsnittet. Ett filter objekt blir tillgängligt om du har data i filter villkoren. 

- Standard valet av varje filter lista är **alla**. Om du till exempel inte har valt en viss produkt i produkt filtret, är standard valet alla produkter.

- Filter som är markerade visas överst på sidan. 

:::image type="content" source="images/pci/filters.png" alt-text="En delvis skärm bild som visar applicerade filter fält med filter val för produkter, kund marknader, partner beskrivare och försäljnings kanaler.":::

### <a name="filters-definitions"></a>Filter definitioner:

- Produkter: lista över alla Microsoft Cloud produkter som säljs/hanteras av din organisation, till exempel O365, Azure, D365, EMS, Power BI osv.
- Kund marknader: lista över kund länder
- Partner rättigheter: din kopplings typ med dina kunders prenumerationer, till exempel digital partner of Record (DPOR), delegerad administratörs behörighet (DAP) och partner admin Link (PAL). 
- Partner platser: lista över alla organisationens MPN-platser.
- Försäljnings kanaler: all försäljnings kanal/prissättning genom vilken du köper/distribuerar produkter och tjänster, nämligen CSP, EA, CSP indirekt, Direct, Advisor, Open, övrigt
- Kund segment: lista över kund segment i partnerns kund bas.

## <a name="read-about-each-of-the-dashboards-and-reports"></a>Läs om var och en av instrument panelerna och rapporterna:

- [Instrument panel för partner Center Insights – översikt](pci-overview-report.md)

- [Partner Center Insights – kund instrument panel](pci-customer-report.md)

- [Partner Center Insights – prenumerations rapport](pci-product-subscriptions-report.md)

- [Partner Center Insights – licens rapport](pci-product-licenses-report.md)

- [Partner Center Insights – Azures användnings rapport](pci-azure-usage-report.md)

- [Partner Center Insights – kompetens rapport](pci-competencies-report.md)

- [Partner Center Insights – förmåns rapport](pci-benefits-report.md)
