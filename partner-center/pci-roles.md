---
title: Partner Center Insights-rollbaserad åtkomst
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig mer om de roller som krävs för att visa rapporter om Partner Center Insights. Dessa inkluderar roller för rapport visnings programmet och rapport visnings programmet.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 980c086a2ab1ee0a21592ceb1e2e018c0e1159ae
ms.sourcegitcommit: bcd0c09d3acd5eae4fbfca7ea6614a54d203eff6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2020
ms.locfileid: "92531396"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Rollbaserad åtkomst kontroll till Partner Center Insights-instrumentpanelen

På instrument panelen för insikter används två nya roller i Partner Center för att hantera medarbetarnas åtkomst till rapport visnings programmet rapporter – Executive och Report Viewer.  Användare i rollen Executive Report Viewer har åtkomst till alla rapporterings data uppsättningar, medan användare i rapport visnings rollen inte har åtkomst till känsliga data uppsättningar, till exempel intäkter och kund/anställdas personliga data.  

Precis som med andra partner Center-roller kommer den globala administratören eller konto administratören att kunna tilldela användare till dessa roller på sidan användar hantering. Rollerna kan tillämpas i hela företaget eller för vissa MPN-platser. Roller som har tilldelats till vissa MPN-platser begränsar användaren till att Visa rapporterings data som endast är kopplade till de valda MPN-platserna. Partner kan välja en eller flera platser i vyn nedan.

:::image type="content" source="images/pci/roles.png" alt-text="Visar inställningar för plats-/regionsspecifika Partner Center Insights-roller för rapport visnings programmet och rapport visnings programmet.":::

>[!Note]
> Användare som är MPN-administratörer från och med den 20 januari 2020 läggs automatiskt till i rollen företags omfattande **rapport visnings program** för alla platser för den klienten. Dessa användare kan därför komma åt rapporterna som ett verk ställande rapport visnings program utan uttryckliga åtgärder som krävs av global administratör eller konto administratör. De globala administratörerna och konto administratörerna kan åsidosätta de automatiskt tilldelade rollerna för dessa användare för att ytterligare öka eller begränsa deras funktioner.

## <a name="next-steps"></a>Nästa steg

- Lär dig mer om [partner Center Insights](partner-center-insights.md) och dess olika rapporter.
