---
title: Hantera din kundlista
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Kundposter är bland de viktigaste informationstillgångarna. Lär dig hur du visar, söker efter, uppdaterar & exporterar information i din Partnercenter-kundlista.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1791d415d0004520e8c7dc950decf540c91cf003
ms.sourcegitcommit: 26e6b470756aa9c1b3b0b919301b0eb38a335a52
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/26/2021
ms.locfileid: "108002849"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Hantera din kundlista – söka efter, uppdatera eller exportera kunder i Partnercenter

**Gäller för**

- Välkommen till Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller**

- Administratörsagent
- Global administratör

Kundposter är bland dina viktigaste informationstillgångar i Partnercenter. Du kan söka i databasen med kundkonton, exportera hela kunddatabasen eller exportera en delmängd till ett Excel-kompatibelt filformat med kommaavgränsade värden (.csv). Du kan också exportera en kunds prenumerationsinformation till en CSV-fil.

Aktivitetsloggar ger också exporterbara data om transaktioner och hanteringsåtgärder för kunder. Mer information finns i Visa [kundaktivitetsloggar.](activity-logs.md)

## <a name="search-for-a-customer"></a>Sök efter en kund

1. I **menyn i Partnercenter** väljer du **Kunder.**
2. Om du vill söka efter en kund anger du kundnamnet eller domännamnet i sökrutan.
3. Välj **nedåtpilen i** slutet av en kundrad för att se deras Microsoft-ID och deras associerade prenumerationer och tjänster snabblänkar.

## <a name="update-a-customers-company-name"></a>Uppdatera en kunds företagsnamn

I **menyn i Partnercenter** väljer du **Kunder.**
2. Om du vill söka efter en kund anger du kundnamnet eller domännamnet i sökrutan.
3. Välj **nedåtpilen i** slutet av en kundrad för att se deras Microsoft-ID och deras associerade prenumerationer och tjänster snabblänkar.
4. Under kundens **faktureringsinformation uppdaterar** du företagets namn. När du sparar det nya värdet visas det i kundlistan. Detta ändrar bara faktureringsföretagets namn och värdet för kundlistan. Den återspeglas inte någon annanstans.

## <a name="export-your-customer-list"></a>Exportera din kundlista

1. I **menyn i Partnercenter** väljer du **Kunder.**
2. Välj **Exportera kunder.**

   Partnercenter konverterar hela kundlistan till en CSV-fil och laddar upp den till standardmappen för nedladdning på datorn. Du kan också exportera delmängder av kunddata. Datakolumner omfattar följande:

   - **Microsoft ID**;
   - **Företagsnamn**;
   - **Primärt domännamn**;
   - **Relation**– partnerns affärsrelation till varje kund i listan.

    Som standard exporterar Partner Center hela kundlistan, oavsett längd. Du kan också söka i kundlistan efter företagsnamn eller domän och exportera den delmängden data.

3. Om du är en indirekt leverantör kan du filtrera kundlistan efter indirekt återförsäljare. Välj **Filtrera efter indirekt återförsäljare** i listan och välj sedan en återförsäljare.


## <a name="export-customer-subscription-information"></a>Exportera information om kundprenumeration

1. I **menyn i Partnercenter** väljer du **Kunder.**

2. Välj **företagsnamnet för** alla kunder. Kundens **prenumerationssida öppnas** och visar en fullständig lista över produktprenumerationer.

3. Välj **Exportera prenumerationer.** PartnerCenter konverterar kundens prenumerationsdata till en CSV-fil och laddar upp dem till standardmappen för nedladdning på datorn. Datakolumner innehåller följande:
   - **Prenumerations-ID**;
   - **Prenumeration**– produktnamnet för prenumerationen;
   - **Kvantitet**– antalet köpta licenser;
   - **Status**;
   - **Reseller**– ID för återförsäljaren som äger och hanterar prenumerationen.

> [!NOTE]  
> Mer information om prenumerationshantering finns i [Kundprenumerationer.](customer-subscriptions.md)
