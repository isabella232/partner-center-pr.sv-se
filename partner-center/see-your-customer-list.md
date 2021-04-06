---
title: Hantera din kundlista
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Kund poster är bland de viktigaste informations till gångarna. Lär dig att visa, söka, uppdatera & exportera information på kund listan i din partner Center.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 244a8cfc661b371b611a19a5c90ddf131b42a46a
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441973"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Hantera din kund lista – Sök, uppdatera eller exportera kunder i Partner Center

**Gäller för**

- Välkommen till Partnercenter för Microsoft Cloud for US Government

Kund poster är bland dina viktigaste informations till gångar i Partner Center. Du kan söka i din databas med kund konton, exportera hela kund databasen eller exportera en delmängd till ett Excel-kompatibelt kommaavgränsat värde fil format (. csv). Du kan också exportera en kunds prenumerations information till en. csv-fil.

Aktivitets loggar tillhandahåller även exporterade data om transaktioner och hanterings åtgärder för kunder. Mer information finns i [Visa kund aktivitets loggar](activity-logs.md).

## <a name="search-for-a-customer"></a>Sök efter en kund

1. Från menyn **partner Center** väljer du **kunder**.
2. Om du vill söka efter en kund anger du kund namnet eller domän namnet i sökrutan.
3. Välj **nedåtpilen i slutet** av en kund rad för att se deras Microsoft-ID och deras associerade prenumerationer och tjänster snabb länkar.

## <a name="update-a-customers-company-name"></a>Uppdatera en kunds företags namn

Från menyn **partner Center** väljer du **kunder**.
2. Om du vill söka efter en kund anger du kund namnet eller domän namnet i sökrutan.
3. Välj **nedåtpilen i slutet** av en kund rad för att se deras Microsoft-ID och deras associerade prenumerationer och tjänster snabb länkar.
4. Uppdatera företags namnet under kundens **fakturerings** information. När du sparar det nya värdet visas det i listan kund. Detta ändrar endast fakturerings företagets namn och kund List värde. Det kommer inte att reflekteras någon annan stans.

## <a name="export-your-customer-list"></a>Exportera din kund lista

1. Från menyn **partner Center** väljer du **kunder**.
2. Välj **Exportera kunder**.

   Partner Center konverterar din fullständiga kund lista till en. csv-fil och laddar upp den till standard katalogen för hämtning på din dator. Du kan också exportera del mängder av kund information. Data kolumnerna innehåller följande:

   - **Microsoft-ID**;
   - **Företags namn**;
   - **Primärt domän namn**;
   - **Relation**– partnerns affärs relation till varje listad kund.

    Som standard exporterar Partner Center hela kund listan, oavsett längd. Du kan också söka i kund listan efter företags namn eller domän och exportera en delmängd av data.

3. Om du är en indirekt leverantör kan du filtrera din kund lista efter indirekt åter försäljare. Välj **Filtrera efter indirekt åter försäljare** i listan och välj sedan en åter försäljare.


## <a name="export-customer-subscription-information"></a>Exportera kund prenumerations information

1. Från menyn **partner Center** väljer du **kunder**.

2. Välj **företags namnet** för vilken kund som helst. Sidan kund **prenumerationer** öppnas och visar en fullständig lista över produkt prenumerationer.

3. Välj **Exportera prenumerationer**. Partner Center konverterar kundens prenumerations data till en CSV-fil och laddar upp den till standard katalogen för hämtning på din dator. Data kolumnerna innehåller följande:
   - **Prenumerations-ID**;
   - **Prenumeration**– produkt namnet för prenumerationen.
   - **Antal**– antal köpta licenser;
   - **Status**;
   - **Åter försäljare**– ID för den åter försäljare som äger och hanterar prenumerationen.

> [!NOTE]  
> Mer information om prenumerations hantering finns i [kund prenumerationer](customer-subscriptions.md).
