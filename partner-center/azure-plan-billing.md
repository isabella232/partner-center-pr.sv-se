---
title: Fakturering för Azure-plan – & rekognoseringsfiler
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Lär dig hur du får åtkomst till och förstår faktura- och avstämningsfilstrukturen som rör fakturering för Azure-planen.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ad04b7af67bb4cf664b2a552c94fc96fa25e5349
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089274"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Ny handelsupplevelse i CSP – Azure-fakturering

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Global administratör

Den här artikeln förklarar hur du kommer åt och förstår faktura- och avstämningsfilstrukturen som rör fakturering för Azure-planen. Fakturering under Azure-planen är en förenklad faktureringsupplevelse med ett justerat faktureringsdatum och kalendermånadsbaserad faktureringsperiod.

## <a name="summary-of-billing-essentials"></a>Sammanfattning av faktureringsinformation

- **Fakturadatum:** Faktura- och avstämningsfilen blir tillgänglig i instrumentpanelen/API:et i Partnercenter den 8:e (midnatt UTC).

- **Faktureringsperiod för** faktura: Faktureringsperioden justeras till kalendermånaden, till exempel 10/1-10/31, 11/1-11/30.

- **Avgiftstjänstperioder:** Avgifterna justeras efter kalendermånaden. Om den fakturerade partnern till exempel lägger till Azure-tjänster via en Azure-plan den 10/15 och kunden börjar använda Azure-tjänster den 10/15 får den fakturerade partnern faktura/rekognosering den 11/8 för kundförbrukning för tjänstperioden 10/15–10/31. Nästa månads faktura som ska genereras den 12/8 innehåller alla avgifter för tjänstperioden 11/1–11/31.

- **Fakturabetalning:** 60 dagar efter.

- **Fakturavaluta:** Från och med augusti 2021 debiteras alla partner i partnerns valuta oavsett var kunden som du sålde produkterna finns.

- **Partnerincitament:** Betalas 45 dagar från slutet av fakturamånaden.

## <a name="access-your-invoices-and-reconciliation-files"></a>Få åtkomst till dina fakturor och avstämningsfiler

Den globala administratören eller faktureringsadministratören för ditt företag får ett e-postmeddelande när en faktura är redo att visas.

Så här kommer du åt faktura- och avstämningsfilen:

> [!NOTE]
> Mer information om gränssnittet för arbetsytor finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vy över arbetsytor](#tab/workspaces-view)

1. På [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/)väljer du **panelen** Fakturering.

2. Välj fliken för **Återkommande och** **Engångs och den** valuta som du är intresserad av.

   :::image type="content" source="images/azure/billing-workspace-1.png" alt-text="Skärmbild som visar faktureringshistorik.":::

3. Välj **Faktura eller** **Avstämningsfil**.

   Om du vill visa historiska fakturor och avstämningsfiler expanderar du raden Faktureringshistorik nedan.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. Från [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/)väljer du **Fakturering.**

2. Välj fliken för **Återkommande och** **Engångs och den** valuta som du är intresserad av.

   :::image type="content" source="images/azure/billing3.png" alt-text="Fakturering.":::

3. Välj **Faktura eller** **Avstämningsfil**.

   Om du vill visa historiska fakturor och avstämningsfiler expanderar du raden Faktureringshistorik nedan.

* * *

## <a name="about-usage-data"></a>Om användningsdata

- Azure-planen är rot- eller toppnivåcontainern för användning. All användning är kopplad till en enda Azure-plan.

- Inom en plan finns det en eller flera Azure-prenumerationer. Det här är containrar som används för resurshantering och distribution.

- I en prenumeration lägger resursgrupper till i gruppresurser. Varje resurs distribueras till en resursgrupp.

- Exempel på resurser är virtuella datorer och lagringskonton.

- Resursavsändarmätare: Mätare är mätningar av förbrukningen för en resurs och en resurs kan generera användning för flera mätare. Mätare identifieras av ett ProductId, SKUId och AvailabilityId.

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hierarki för prenumerationsresursgrupper och mätning

**Azure-konto (klient)**

- Prenumeration A
    - ResourceGroup 1
        - Virtuell dator (resurs)
            - Beräkningsmätare
        - Virtuellt nätverk (resurs)
            - Ingen faktureringsmätare

    - ResourceGroup 2
        - Virtuell dator (resurs)
            - Datormätare
        - Premium SSD-hanterad disk (resurs)
            - Storage kapacitetsmätare
            - Storage driftmätare

- Prenumeration B -ResourceGroup 1 – Azure SQL (resurs) – DTU-mätare – VPN Gateway (resurs) – VPN-gatewaymätare

    - ResourceGroup 2
        - Virtual Network (resurs)
            - Ingen faktureringsmätare

## <a name="about-your-invoice"></a>Om din faktura

- Fakturan blir tillgänglig senast den åttonde i varje månad.

- Partner har 60 dagar på sig att betala.

- Faktureringsperioden omfattar en viss kalendermånad, till exempel 10/1-10/31.

- Avgifterna är nettojusteringar (beloppet är efter "Partner-intjänad kredit för hanterade tjänster").

- Granska fakturans rekognoseringsfil och filen med daglig klassificerad användning för ytterligare faktureringsinformation.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Faktura.":::

## <a name="about-your-invoice-reconciliation-file"></a>Om din fakturaavstämningsfil

- Varje kombination av Azure-plan och mätare kan ha upp till två faktureringsrader i avstämningsfilen (recon).

- Om mätaren är kvalificerad för någon typ av rabatt eller kredit (till exempel nivåindelade rabatter eller partner-intjänad kredit för tjänster som hanteras) under hela kalendermånaden innehåller rekognoseringsfilen endast en faktureringsrad. Kolumnen **PriceAdjusmentDescription refererar till** rabatten eller intjänad kredit.

- Om det inte finns några resurser för en viss mätare som är kvalificerade för rabatt eller partner-intjänad kredit innehåller rekognoseringsfilen bara en faktureringsrad och det effektiva enhetspriset är detaljhandelspriset (vilket är enhetspriset).

- Om mätaren, eller resurser som sänder  mätaren, är kvalificerad för partner-intjänad kredit för tjänster som hanteras under en del av månaden, innehåller rekognoseringsfilen två faktureringsrader. En rad representerar de dagar då mätaren kvalificerades och den andra raden representerar de dagar då mätaren inte var kvalificerad.

> [!NOTE]
> Du kan stämma av Din Azure-förbrukning i rekognoseringsfilen för ett köp en gång. Det gör du genom att gå till din dagliga avsökningsfil för användning och söka efter ditt SubscriptionID. Då visas alla kostnader som är kopplade till ditt Azure-plan-ID. Ditt Azure SubscriptionID visas som EntitlementID.

## <a name="read-the-daily-usage-file"></a>Läsa filen för daglig användning

- Prenumerationsmätare under en Azure-plan klassificeras och ackumuleras dagligen.

- **Partnerns intjänade kredit för** tjänster som hanteras fastställs och tillämpas dagligen.

- Varje prenumerationsmätare har en rad för varje dag i månaden där det fanns förbrukning.

- I exemplet nedan:

  - Mätare som är kvalificerad för partner-intjänad kredit för tjänster som hanteras från 7/1 till 7/3 (observera att det effektiva enhetspriset är återförsäljarpris minus partner-intjänad kredit. 

  - Meter var inte  kvalificerat för partner-intjänad kredit för tjänster som hanteras 7/4–7/7 (observera att det effektiva enhetspriset är återförsäljarpris).

  - Mätare som är kvalificerad för partner-intjänad kredit för tjänster som hanteras från 7/8 till 7/31 (observera att det effektiva enhetspriset är återförsäljarpris minus partners intjänade kredit). 

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-partner-location-currency"></a>Faktura i partnerns platsvaluta

Azure-tjänster via en Azure-plan prissätts i USD och faktureras i partnerns tilldelade valuta. Om faktureringsvalutan inte är USD visas den valutakurs (FX) som används på den sista sidan på fakturan. FX-priser bestäms varje månad och tillämpas på följande faktura. En fullständig lista över länders valutor finns i den nya handelslösningen med [landstillgänglighet och partnervalutamatrisen](https://go.microsoft.com/fwlink/?linkid=2112354).

Microsoft tillämpar en förutbestämd växelkurs för att basera USD-priser för att komma fram till de totala avgifter som tillkommer för Azure-tjänster som köpts eller förbrukats varje kalendermånad. Den månatliga växelkursen är den genomsnittliga kursen som publiceras av AntenPrise (vanligtvis) två arbetsdagar före den föregående månadens slut kl. 16:00 GMT.

**Till exempel** Microsofts växlingskurs i december skulle vara Det medelstora priset För en viss valuta den 29 november eller runt den 29 november. Den kursen tillämpas på alla inköp i den valutan från 1 december till 31 december.

## <a name="azure-reservations"></a>Azure-reservationer

Om du [köper Azure-reservationer](azure-reservations.md) via en Azure-plan kan du välja antingen en gång eller månatlig fakturering.

## <a name="azure-spending"></a>Utgift i Azure

Den befintliga Azure-utgiftsupplevelsen har uppdaterats för att stödja den nya Azure-planfakturering i Partnercenter. Detta gör att partner kan:

- Visa, hantera och ta emot aviseringar för budget som angetts på kundnivå

- Visa totala beräknade utgifter för en Azure-plan (uppdelade efter resurs- och mätarnivå)

Eftersom faktureringsmodellen för Azure-tjänster via en Azure-plan är förbrukning efter betalning kan partner använda en månatlig budget och spåra procentandelen av användningen för att undvika en större faktura än förväntat. En budget kan tillämpas på en kund eller flera kunder i taget.

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure-utgifter.":::

## <a name="next-steps"></a>Nästa steg

- Se hur partnerns intjänade kredit (PEC) beräknas. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/) och välj panelen **Prissättning för** att hitta tillgängliga prislistor.

- Lär dig mer [om att köpa Azure-planen](purchase-azure-plan.md)

- Se [prislistan för den nya handelsupplevelsen i CSP](azure-plan-price-list.md)
