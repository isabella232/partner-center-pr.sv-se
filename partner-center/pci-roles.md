---
title: Partner Center Insights rollbaserad åtkomst
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig mer om de specifika roller som behövs för att se Partner Center Insights-rapporter. Dessa inkluderar rollerna Executive Report Viewer och Report Viewer.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 803c299311f129c4842a92a27abd9b9addb49f17
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854442"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Rollbaserad åtkomstkontroll till instrumentpanelen i Partner Center Insights

**Lämpliga roller:** Global | Administratörsagent | Rapportvisningsprogram | Rapportvisningsprogram för chefer

Instrumentpanelen Insikter använder två nya roller i Partnercenter för att hantera medarbetarnas åtkomst till rapporterna – Visningsprogrammet för chefsrapport och Rapportvisningsprogrammet.  Användare i rollen Visningsprogram för verkställande rapporter har åtkomst till alla rapportdatamängder, medan användare i rollen Rapportvisningsprogram inte har åtkomst till känsliga datauppsättningar, till exempel intäkter och kund-/medarbetares personliga data.  

Precis som med andra Partnercenter-roller kommer den globala administratören eller kontoadministratören att kunna tilldela användare till dessa roller på sidan Användarhantering. Rollerna kan tillämpas på hela företaget eller för specifika MPN-platser. Roller som tilldelats för specifika MPN-platser begränsar användaren till att visa rapportdata som endast är associerade med de valda MPN-platserna. Partner kan välja en eller flera platser i vyn nedan.

:::image type="content" source="images/pci/roles.png" alt-text="Visar platsspecifika inställningar för Partner Center Insights-roller för rapportvisningsprogrammet och rapportvisningsprogrammet för chefer.":::

>[!Note]
> Användare som är MPN-administratörer från och med den 20 januari 2020 läggs automatiskt till i rollen Executive **Report Viewer** för hela företaget för alla platser för den klientorganisationen. Dessa användare kan därför komma åt rapporterna som visningsprogram för verkställande rapporter utan uttryckliga åtgärder som krävs av global administratör eller kontoadministratör. Globala administratörer och kontoadministratörer kan åsidosätta de automatiskt tilldelade rollerna för dessa användare för att ytterligare öka eller begränsa deras funktioner.

## <a name="next-steps"></a>Nästa steg

- Läs mer om [Partner Center Insights](partner-center-insights.md) och dess olika rapporter.
