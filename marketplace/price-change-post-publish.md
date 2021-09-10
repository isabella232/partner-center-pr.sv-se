---
title: Prisändringar i Marketplace-produkter efter publicering
description: I den här artikeln beskrivs vanliga frågor om att ändra priser på planer efter publicering.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 08/27/2021
ms.openlocfilehash: bfb99986483d0aaaa5d685c266c8118c1345517c
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123936977"
---
# <a name="price-changes-to-marketplace-products"></a>Prisändringar för Marketplace-produkter

Oberoende programvaruleverantörer (ISV: er) som säljer sina produkter via Azure Marketplace kan uppdatera planpriser (eller SKU:er) då och då. Det nya priset för SKU:n kan vara högre eller lägre än det tidigare priset. Prisändringen uppdateras på produkt-/SKU-/marknadsnivå. Därför kan det finnas prisuppdateringar som är relevanta för vissa marknader, men inte för alla.

I vissa fall (se nedan) kan prisändringen påverka produkter som har köpts tidigare och kunden ser en prisändring på månadsfakturan. Azure Marketplace kunder som använder dessa produkter minst 90 dagar innan det nya priset börjar gälla.

## <a name="which-offer-types-can-be-affected-from-price-change"></a>Vilka erbjudandetyper kan påverkas av prisändringen?

Alla köpbara produkter som säljs via Azure Marketplace och AppSource, till exempel produkter som har en eller flera planer.

## <a name="can-a-free-sku-turn-one-day-into-a-paid-one"></a>Kan en kostnadsfri SKU bli en dag till en betald?

Nej. ISV:n kan inte omvandla en kostnadsfri SKU till en betald SKU. En ISV som vill göra en produkt fakturerbar måste publicera en ny betald SKU.

## <a name="price-increase-awareness-in-the-marketplace-product-pages"></a>Prisökningsmedvetenhet på produktsidor på Marketplace

Som tidigare nämnts måste ISV:er som vill publicera en prisökning ge minst 90 dagars varning innan det nya priset börjar gälla. Detta är för att ge meddelanden till kunder som planerar att köpa en produkt. Marketplace-produktsidor uppdateras minst 90 dagar i förväg om den kommande ändringen. Sidorna uppdateras med ett meddelande som beskriver det kommande datumet för prisändringen och det nya priset

:::image type="content" source="media/price-change/plan-pricing.png" alt-text="Visar prissidan för planen":::

> [!NOTE]
> Prissättningen i bilden ovan är endast i exempelsyfte. Faktiska priser kan variera.

Ett sådant meddelande visas bara om priset går upp och inte om priset går ned.

## <a name="when-is-the-new-price-taking-effect"></a>När gäller det nya priset?

 Det nya effektiva priset kommer alltid att vara i början av en kalendermånad. Med 90-dagarsperioden ser en typisk tidslinje för prisuppdatering ut så här:

Jan-15 – ISV uppdaterar en framtida prisuppdatering till en SKU i katalogen

16 januari–18 januari – produktsidan uppdateras med ett varningsmeddelande om kommande prisökningar som börjar den 1 maj (slutet av januari + 90 dagar).

1 maj – det nya priset gäller

## <a name="customers-affected-from-a-price-change-post-purchase"></a>Kunder som påverkas av en prisändring (efter köpet)

Att köpa en produkt före det effektiva datumet för *prisökningen garanterar* inte inköpspriset under hela produktdistributionen. Olika typer av erbjudanden som påverkas är:

- Förbrukningsbaserade produkter (till exempel virtuella datorer som debiteras per timme eller priset för förbrukningsbaserad användning av SaaS eller hanterat apperbjudande) när det nya priset är effektivt ökar kostnaden för förbrukningsenhet. För kunder som debiteras i mitten av månaden finns det två rader i rapporten för månatlig användning: en för förbrukning fram till det nya effektiva priset (i exemplet ovan: 1 maj) och en för förbrukning efter det effektiva datumet
- Förbrukningsbaserade produkter med månadsavgift (till exempel SaaS med anpassade mätare), påverkas förbrukningsenheters pris när det nya priset börjar gälla på marknadsplatsen. Månadsavgiften hålls oförändrad fram till slutet av rättighetsperioden.
- Seat-baserade produkter (till exempel licensbaserade SaaS-tjänster), om prisändringens effektiva datum inträffar efter köpet garanteras inköpspriset fram till nästa förnyelsedatum, om det är månatlig förnyelse eller årlig förnyelsedatum.
    - Tillägg eller borttagning av platser efter det datum då priset ändrades, men före förnyelsedatumet för kontraktet, behålls till det ursprungliga inköpspriset. Vid förnyelsen börjar det nya priset gälla.
    - Ändring av SKU, ändring av SKU efter det effektiva datumet för prisändringen betraktas som ett nytt köp och kommer att omfattas av det nya priset. Den här ändringen gäller även scenarier där ändring av antalet platser kräver att kundens SKU ändras. Du kan till exempel flytta från 400 till 500 platser, vilket kan kräva att kunden köper en ny nivå/SKU för produkten.

## <a name="customer-notifications"></a>Kundmeddelanden

Kunder som redan använder produkten/SKU:n på en marknad som påverkas av den kommande prisökningen meddelas via e-post om den kommande ändringen. Detta är så att de kan vidta åtgärder om de vill göra det. E-postmeddelandet skickas 90 dagar innan det nya priset börjar gälla och ett andra meddelande skickas 30 dagar innan prisändringen börjar gälla. Meddelandet skickas till fakturaavsnittsägaren (projektet), faktureringsgruppens ägare och faktureringskontoägare för prenumerationen.

## <a name="next-steps"></a>Nästa steg

- [Vad är Azure Marketplace?](azure-marketplace-overview.md)
- [Azure Marketplace köp](azure-purchasing-invoicing.md)