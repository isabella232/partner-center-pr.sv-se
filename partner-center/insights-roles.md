---
title: Partnercenter Insights rollbaserad åtkomst
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Lär dig mer om de specifika roller som behövs för att se Partnercenter Insights rapporter. Dessa omfattar rollerna Executive Report Viewer och Report Viewer.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 91bb81fce340a945d9b6e43277d06156a03f1db1
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836327"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Rollbaserad åtkomstkontroll till Partnercenter Insights instrumentpanel

**Lämpliga roller:** Globala | Administratörsagent | Rapportvisningsprogram | Visningsprogram för exekutiv rapport

Instrumentpanelen Insights två nya roller i Partnercenter för att hantera medarbetares åtkomst till rapporterna – Visningsprogrammet för exekutiv rapport och rapportvisningsprogrammet.  Användare i rollen Visningsprogram för verkställande rapporter har åtkomst till alla rapportdatamängder, medan användare i rollen Rapportvisning inte har åtkomst till känsliga datauppsättningar, till exempel intäkter och kund-/medarbetares personliga data.  

Precis som med andra Partnercenter-roller kommer den globala administratören eller kontoadministratören att kunna tilldela användare till dessa roller på sidan Användarhantering. Rollerna kan tillämpas på hela företaget eller för specifika Microsoft Partner Network (MPN)-platser. Roller som tilldelats för specifika MPN-platser begränsar användaren till att visa rapportdata som endast är associerade med de valda MPN-platserna. Partner kan välja en eller flera platser i vyn nedan.

:::image type="content" source="images/insights/roles.png" alt-text="Visar platsspecifika partnercenterinställningar Insights rapportvisningsprogrammet och rapportvisningsprogrammet.":::

>[!Note]
> Användare som är MPN-partneradministratörer från och med den 20 januari 2020 läggs automatiskt till i rollen Executive **Report Viewer** för hela företaget för alla platser för den klientorganisationen. Dessa användare kan därför komma åt rapporterna som visningsprogram för exekutiv rapport utan uttryckliga åtgärder som krävs av global administratör eller kontoadministratör. Globala administratörer och kontoadministratörer kan åsidosätta de automatiskt tilldelade rollerna för dessa användare för att ytterligare öka eller begränsa deras funktioner.

## <a name="next-steps"></a>Nästa steg

- Läs mer om [PartnerCenter Insights](partner-center-insights.md) och dess olika rapporter.
