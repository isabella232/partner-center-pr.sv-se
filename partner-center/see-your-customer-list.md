---
title: Hantera din kundlista
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Kundposter är bland de viktigaste informationstillgångarna. Lär dig hur du visar, söker efter, uppdaterar & exporterar information i din Partnercenter-kundlista.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d98a6a786f63218051fb2d781153c05d8383b4eb
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129075077"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Hantera din kundlista – söka efter, uppdatera eller exportera kunder i Partnercenter

**Gäller för:** Partner Center | Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller:** Administratörsagent | Global administratör

Kundposter är bland dina viktigaste informationstillgångar i Partnercenter. Du kan söka i databasen med kundkonton, exportera hela kunddatabasen eller exportera en delmängd till ett Excel-kompatibelt filformat med kommaavgränsade värden (.csv). Du kan också exportera en kunds prenumerationsinformation till en .csv fil.

Aktivitetsloggar ger också exporterbara data om transaktioner och hanteringsåtgärder för kunder. Mer information finns i Visa [kundaktivitetsloggar.](activity-logs.md)

## <a name="search-for-a-customer"></a>Sök efter en kund

#### <a name="workspaces-view"></a>[Vy över arbetsytor](#tab/workspaces-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard) och välj **panelen** Kunder.
2. Ange kundens namn eller domännamn i sökrutan.
3. Välj **nedåtpilen i** slutet av en kundrad för att se deras Microsoft-ID och deras associerade prenumerationer och tjänster snabblänkar.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. I **menyn i Partnercenter** väljer du **Kunder.**
2. Om du vill söka efter en kund anger du kundnamnet eller domännamnet i sökrutan.
3. Välj **nedåtpilen i** slutet av en kundrad för att se deras Microsoft-ID och deras associerade prenumerationer och tjänster snabblänkar.

* * *

## <a name="update-a-customers-company-name"></a>Uppdatera en kunds företagsnamn

#### <a name="workspaces-view"></a>[Vy över arbetsytor](#tab/workspaces-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard) och välj **panelen** Kunder.
2. Ange kundens namn eller domännamn i sökrutan.
3. Välj **nedåtpilen i** slutet av en kundrad för att se deras Microsoft-ID och deras associerade prenumerationer och tjänster snabblänkar.
4. Under kundens **faktureringsinformation uppdaterar** du företagets namn. När du sparar det nya värdet visas det i kundlistan. Detta ändrar bara faktureringsföretagets namn och kundlistans värde. Den återspeglas inte någon annanstans.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

I **menyn i Partnercenter** väljer du **Kunder.**
2. Om du vill söka efter en kund anger du kundnamnet eller domännamnet i sökrutan.
3. Välj **nedåtpilen i** slutet av en kundrad för att se deras Microsoft-ID och deras associerade prenumerationer och tjänster snabblänkar.
4. Under kundens **faktureringsinformation uppdaterar** du företagets namn. När du sparar det nya värdet visas det i kundlistan. Detta ändrar bara faktureringsföretagets namn och kundlistans värde. Den återspeglas inte någon annanstans.

* * *

## <a name="export-your-customer-list"></a>Exportera din kundlista

#### <a name="workspaces-view"></a>[Vy över arbetsytor](#tab/workspaces-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard) och välj **panelen** Kunder.
2. Välj **Exportera kunder.**

   PartnerCenter konverterar din fullständiga kundlista till en .csv-fil och laddar ned den till standardmappen för nedladdning på datorn. Du kan också exportera delmängder av kunddata. Datakolumner innehåller följande:

   - **Microsoft ID**;
   - **Företagsnamn**;
   - **Primärt domännamn**;
   - **Relation**– partnerns affärsrelation till varje kund i listan.

    Som standard exporterar Partner Center hela kundlistan, oavsett längd. Du kan också söka i kundlistan efter företagsnamn eller domän och exportera den delmängden data.

3. Om du är en indirekt leverantör kan du filtrera din kundlista efter indirekt återförsäljare. Välj **Filtrera efter indirekt återförsäljare** i listan och välj sedan en återförsäljare.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. I **menyn i Partnercenter** väljer du **Kunder.**
2. Välj **Exportera kunder.**

   Partner Center konverterar din fullständiga kundlista till en .csv fil och laddar upp den till standardmappen för nedladdning på datorn. Du kan också exportera delmängder av kunddata. Datakolumner innehåller följande:

   - **Microsoft ID**;
   - **Företagsnamn**;
   - **Primärt domännamn**;
   - **Relation**– partnerns affärsrelation till varje kund i listan.

    Som standard exporterar Partner Center hela kundlistan, oavsett längd. Du kan också söka i kundlistan efter företagsnamn eller domän och exportera den delmängden data.

3. Om du är en indirekt leverantör kan du filtrera din kundlista efter indirekt återförsäljare. Välj **Filtrera efter indirekt återförsäljare** i listan och välj sedan en återförsäljare.

* * *

## <a name="export-customer-subscription-information"></a>Exportera information om kundprenumeration

1. I **menyn i Partnercenter** väljer du **Kunder.**

2. Välj **Företagsnamn för** alla kunder. Kundens **prenumerationssida öppnas** och visar en fullständig lista över produktprenumerationer.

3. Välj **Exportera prenumerationer.** Partner Center konverterar kundens prenumerationsdata till en .csv och laddar upp den till standardmappen för nedladdning på datorn. Datakolumner innehåller följande:
   - **Prenumerations-ID**;
   - **Prenumeration**– produktnamnet för prenumerationen;
   - **Kvantitet**– antalet köpta licenser;
   - **Status**;
   - **Reseller**– ID för den återförsäljare som äger och hanterar prenumerationen.

> [!NOTE]  
> Mer information om prenumerationshantering finns i [Kundprenumerationer.](customer-subscriptions.md)
