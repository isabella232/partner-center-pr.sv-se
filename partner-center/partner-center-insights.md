---
title: Partnercenter Insights
description: Utforska den här enhetliga rapportinstrumentpanelen i Partnercenter. Se hur det går för dig i KPI:er för försäljning och distribution, kundutveckling med mera.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: 46a15d9f26421b78022e15090a5c498f956fb49dce688264074788be88d04cf2
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115696314"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a>PartnerCenter Insights – en instrumentpanel som visar hur det går för en kommersiell Microsoft-partner

**Lämpliga roller:** Globala | Kontoadministratörsbehörighet | Rapportvisningsprogram | Rapportvisningsprogram

## <a name="introduction"></a>Introduktion

Instrumentpanelen Insights är en enhetlig rapportinstrumentpanel i Partnercenter för Microsofts kommersiella partner som är registrerade i programmet Microsoft Partner Network (MPN). I Insights-instrumentpanelen finns en 360-gradig vy över kpi:er för molnprodukter som Office, Azure, Dynamics och licensieringsmodeller som CSP och EA. Den visar en omfattande uppsättning KPI-rapporter som kan hjälpa dig att fatta datadrivna beslut för din organisation. 

## <a name="role-based-access-control-to-the-insights-dashboard"></a>Rollbaserad åtkomstkontroll till Insights instrumentpanel

Det finns två nya roller i Partnercenter som utformats specifikt för åtkomst Insights: **Rapportvisningsprogram** och **Visningsprogram för rapporter.** Användare i rollen Visningsprogram för verkställande rapporter har åtkomst till alla rapportdatamängder, medan användare i rollen Rapportvisning inte har åtkomst till känsliga datauppsättningar, till exempel intäkter och kund-/medarbetares personliga data. 

Den globala administratören eller kontoadministratören kan tilldela användare dessa roller och tilldelas antingen för hela företaget eller för en specifik MPN-plats.  

>[!Note] 
>Användare som var MPN-administratörer den 20 januari 2020 lades automatiskt till i rollen som rapportvisningsprogram för hela företaget. De kan komma åt rapporterna som rapportvisningsprogram utan uttryckliga åtgärder som krävs av global administratör eller kontoadministratör. Globala administratörer eller kontoadministratörer kan åsidosätta dessa tilldelningar om det behövs. 

## <a name="reports-available"></a>Tillgängliga rapporter

Följande rapporter är tillgängliga som en del av Insights instrumentpanel.

**Översikt:** Översiktsrapporten visar en ögonblicksbild av olika KPI:er av intresse för dig, till exempel Antal kunder, Antal aktiva prenumerationer, Azure Consumption Revenue, Aktiva licenser osv.

**Kund:** Kundrapporten visar analyser kring dina kunder, till exempel kundförvärvsdata, aktiva kunder osv.

**Produkt – Prenumerationer:** Prenumerationsrapporten visar förvärvs- och användningsanalys för dina molnprenumerationer (till exempel O365, Azure, Dynamics osv.)

**Produkt – Licenser:** Instrumentpanelen Licenser visar licensanalys för licensbaserade molnprodukter som O365, Dynamics Power BI osv.

**Produkt – Azure-användning:** Azure-användningsrapporten visar mått relaterade till dina kunders Azure-prenumerationer, inklusive Azure-förbrukningsintäkter och -användning efter mätarkategorier.

**Kompetenser:** Rapporten Kompetenser visar mått för dina aktiva, kvalificerade och riskfyllda kompetenser.

**Fördelar:** I rapporten Fördelar visas analys av partnerförmåner som du har intjänat jämfört med förbrukat.

## <a name="navigating-the-insights-reports"></a>Navigera i Insights rapporter

**Datumintervallfilter:** Du hittar ett datumintervall i det övre högra hörnet på varje sida. Du kan anpassa utdata från översiktssidans diagram genom att välja ett datumintervall baserat på de senaste 3, 6 eller 12 månaderna eller genom att välja ett anpassat datumintervall. Standardvalet av datumintervall är 12 månader. 

:::image type="content" source="images/insights/introduction.png" alt-text="Introduktionskarta.":::

**Feedbackknapp:** Varje diagram/kontroll i alla Insights ingår med en feedback-knapp så att du kan ge instansfeedback om en rapportfunktion. 

 
**Sidnivåfilter:** Med undantag för rapporterna Översikt, Förmåner och Kompetenser kan Insights använda filter på sidnivå. 

- De filter som valts gäller för alla diagram och mått på en sida, inklusive sammanfattningsavsnittet. Ett filterobjekt är tillgängligt om du har några data inom filtervillkoren. 

- Standardvalet för varje filterlista är **alla**. Om du till exempel inte har valt en specifik produkt i produktfiltret är standardvalet alla produkter.

- Filter som valts visas överst på sidan. 

:::image type="content" source="images/insights/filters.png" alt-text="Partiell skärmbild som visar fält för tillämpade filter med filterval för produkter, kund marknader, partnerattributioner och försäljningskanaler.":::

### <a name="filters-definitions"></a>Filterdefinitioner:

- Produkter: Lista över alla Microsoft Cloud-produkter som säljs/hanteras av din organisation, till exempel O365, Azure, D365, EMS, Power BI osv.
- Kund marknader: Lista över kund länder
- Partnerattributions: Din associationstyp med dina kunders prenumerationer, till exempel Digital partner of record (DPOR), Delegerad administratörsbehörighet (DAP) och partneradministratörslänk (PAL). 
- Partnerplatser: Lista över organisationens MPN-platser.
- Försäljningskanaler: Alla försäljningskanaler/priser genom vilka du köper/etablerar produkter och tjänster, nämligen CSP, EA, CSP indirect, Direct, Advisor, Open, others
- Kundsegment: Lista över kundsegment mellan partnerkundbasen.

## <a name="read-about-each-of-the-dashboards-and-reports"></a>Läs om var och en av instrumentpanelerna och rapporterna:

- [Partnercenter – Insights – översiktsinstrumentpanel](insights-overview-report.md)

- [Partnercenter – Insights – Kundens instrumentpanel](insights-customer-report.md)

- [Partnercenter – Insights – Prenumerationsrapport](insights-product-subscriptions-report.md)

- [Partnercenter Insights – licensrapport](insights-product-licenses-report.md)

- [Partnercenter Insights – Användningsrapport för Azure](insights-azure-usage-report.md)

- [Partnercenter Insights – kompetensrapport](insights-competencies-report.md)

- [Partnercenter Insights – benefits-rapport](insights-benefits-report.md)
