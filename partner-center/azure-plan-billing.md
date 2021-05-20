---
title: Fakturering av Azure-plan – & rekognoseringsfiler
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du får åtkomst till och förstår strukturen för faktura- och avstämningsfiler relaterade till fakturering för Azure-planen.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ab086a4d15d16f094e33d19b81f1c93711916dc
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201433"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Ny handelsupplevelse i CSP – Azure-fakturering 

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Global administratör

Den här artikeln förklarar hur du kommer åt och förstår strukturen för faktura- och avstämningsfiler relaterade till fakturering för Azure-planen. Fakturering enligt Azure-planen är en förenklad faktureringsupplevelse med ett justerat enskilt faktureringsdatum och kalendermånadsbaserad faktureringsperiod.

## <a name="summary-of-billing-essentials"></a>Sammanfattning av faktureringsinformation

- **Fakturadatum:** Faktura- och avstämningsfilen blir tillgänglig i Partnercenter-instrumentpanelen/API:et den 8:e (midnatt UTC).

- **Faktureringsperiod för** faktura: Faktureringsperioden justeras till kalendermånaden, till exempel 10/1-10/31, 11/1-11/30.

- **Avgiftstjänstperioder:** Avgifterna justeras efter kalendermånaden. Om den fakturerade partnern till exempel lägger till Azure-tjänster via en Azure-plan den 10/15 och kunden börjar använda Azure-tjänster den 10/15, får den fakturerade partnern faktura/rekognosering den 11/8 för kundförbrukning för tjänstperioden 10/15–10/31. Nästa månads faktura som genereras den 12/8 innehåller alla avgifter för tjänstperioden 11/1–11/31.

- **Fakturabetalning:** 60 dagar netto.

- **Fakturavaluta:** Från och med 28 januari 2021 debiteras partner i regionen EU/EFTA och Storbritannien som har nya kunder och befintliga CSP-kunder som köper nya handelserbjudanden för första gången vars klienter skapades före den 11 maj 2020. Partner som är belägna utanför EU/EFTA- och Storbritannien-regionen fortsätter att debiteras i partnerns platsvaluta.

- **Partnerincitament:** Betalas 45 dagar från slutet av fakturamånaden.

## <a name="access-your-invoices-and-reconciliation-files"></a>Få åtkomst till dina fakturor och avstämningsfiler

Den globala administratören eller faktureringsadministratören för ditt företag får ett e-postmeddelande när en faktura är redo att visas.

Så här kommer du åt fakturan och avstämningsfilen:

1. Logga in i Partnercenter och gå till [instrumentpanelen](https://partner.microsoft.com/dashboard/).

2. I menyn i Partnercenter väljer du **Fakturering.**

3. Välj fliken för **Återkommande och** **Engångs och den** valuta som du är intresserad av.

   :::image type="content" source="images/azure/billing3.png" alt-text="Fakturering":::

4. Välj **Faktura eller** **Avstämningsfil**.  

   Om du vill visa historiska fakturor och rekognoseringsfiler expanderar du raden Faktureringshistorik nedan.

## <a name="understanding-usage-data"></a>Förstå användningsdata 

1. Azure-planen är rot- eller toppnivåcontainern för användning. All användning är kopplad till en enda Azure-plan.

2. Inom en plan finns det en eller flera Azure-prenumerationer. Det här är containrar som används för resurshantering och distribution. 

3. I en prenumeration lägger resursgrupper till i gruppresurser. Varje resurs distribueras till en resursgrupp. 

4. Exempel på resurser är virtuella datorer och lagringskonton. 

5. Resursavsändarmätare: Mätare är mätningar av förbrukningen för en resurs och en resurs kan generera användning för flera mätare. Mätare identifieras av ett ProductId, SKUId och AvailabilityId. 

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
        - Premium SSD hanterad disk (resurs)
            - Lagringskapacitetsmätare
            - Mätare för lagringsåtgärder

- Prenumeration B – ResourceGroup 1 – Azure SQL (resurs) – DTU-mätare – VPN Gateway (resurs) – VPN-gatewaymätare

    - ResourceGroup 2
        - Virtual Network (resurs)
            - Ingen faktureringsmätare

## <a name="read-the-invoice"></a>Läsa fakturan

1. Fakturan blir tillgänglig senast den åttonde i varje månad.

2. Partner har 60 dagar på sig att betala.

3. Faktureringsperioden omfattar en viss kalendermånad, till exempel 10/1-10/31.

4. Avgifterna är nettojusteringar (beloppet är netto efter "Partner-intjänad kredit för hanterade tjänster").

5. Granska fakturans rekognoseringsfil och den dagliga klassificerade användningsfilen för ytterligare faktureringsinformation.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Faktura":::

## <a name="read-the-invoice-reconciliation-file"></a>Läsa fakturaavstämningsfilen

1. Varje kombination av Azure-plan och mätare kan ha upp till två faktureringsrader i rekognoseringsfilen.

2. Om mätaren är kvalificerad för någon typ av rabatt eller kredit (till exempel nivåindelade rabatter eller partnerintjänad kredit för tjänster som hanteras) under hela kalendermånaden innehåller rekognoseringsfilen endast en faktureringsrad. Kolumnen **PriceAdjusmentDescription refererar till** rabatten eller den intjänade krediten.

3. Om det inte finns några resurser för en viss mätare som är kvalificerade för rabatt eller partner-intjänad kredit innehåller rekognoseringsfilen bara en faktureringsrad och det effektiva enhetspriset är detaljhandelspriset (vilket är enhetspriset).

4. Om mätaren, eller några resurser som  sänder mätaren, är kvalificerad för partner-intjänad kredit för tjänster som hanteras under en del av månaden, innehåller rekognoseringsfilen två faktureringsrader. En rad representerar de dagar då mätaren kvalificerades och den andra raden representerar de dagar då mätaren inte var kvalificerad.

>[!NOTE]
>Du kan stämma av din Azure-förbrukning i rekognoseringsfilen för ett köp en gång. Det gör du genom att gå till din dagliga avsökningsfil för användning och söka efter ditt SubscriptionID. Då visas alla kostnader som är kopplade till ditt Azure-plan-ID. Ditt Azure SubscriptionID visas som EntitlementID.

## <a name="read-the-daily-usage-file"></a>Läsa filen för daglig användning

- Prenumerationsmätare under en Azure-plan klassificeras och ackumuleras dagligen.

- **Partnerns intjänade kredit för** tjänster som hanteras fastställs och tillämpas dagligen.

- Varje prenumerationsmätare har en rad för varje dag i månaden där det fanns förbrukning.

- I exemplet nedan:

  - Mätare som är kvalificerade för partner-intjänad kredit för tjänster som hanteras från 7/1 till 7/3 (observera att det effektiva enhetspriset är återförsäljarpris minus partner-intjänad kredit. 

  - Meter var inte  kvalificerat för partner-intjänad kredit för tjänster som hanteras 7/4–7/7 (observera att det effektiva enhetspriset är återförsäljarpris).

  - Mätare som är **kvalificerad för partner-intjänad** kredit för tjänster som hanteras från 7/8 till 7/31 (observera att det effektiva enhetspriset är återförsäljarpris minus partners intjänade kredit).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a>Faktura i kundvaluta

Azure-tjänster via en Azure-plan prissätts i USD och faktureras i kundens landstilldelade valuta. Om faktureringsvalutan inte är USD visas det valutautbytespris (FX) som används på den sista sidan på fakturan. FX-priser bestäms varje månad och tillämpas på följande faktura. En fullständig lista över valutor för länder finns i den nya handelslösningen med [landstillgänglighet och kundvalutamatrisen](https://go.microsoft.com/fwlink/?linkid=2112354).

Microsoft följer London-börsen för konvertering. Vi använder växelkursen, som är lika med växelkursen som avbildades den sista sekunden av den sista arbetsdagen i månaden på London-börsen. FX-priserna uppdateras och är tillgängliga dagen före den första i månaden som de gäller för.

## <a name="azure-reservations"></a>Azure-reservationer


Om du [köper Azure-reservationer](azure-reservations.md) via en Azure-plan kan du välja antingen en gång eller månatlig fakturering.


## <a name="azure-spending"></a>Utgift i Azure

Den befintliga Azure-utgiftsupplevelsen har uppdaterats för att stödja den nya Azure-planfakturering i Partnercenter. Detta gör att partner kan:

- Visa, hantera och ta emot aviseringar för budget som angetts på kundnivå 

- Visa totala beräknade utgifter för en Azure-plan (uppdelade efter resurs- och mätarnivå)

Eftersom faktureringsmodellen för Azure-tjänster via en Azure-plan är förbrukning efter betalning kan partner använda en månatlig budget och spåra procentandelen av användningen för att undvika en större faktura än förväntat. En budget kan tillämpas på en kund eller flera kunder i taget. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Utgift i Azure":::

## <a name="next-steps"></a>Nästa steg

- Se hur partnerns intjänade kredit (PEC) beräknas. Logga in på instrumentpanelen [i Partnercenter](https://partner.microsoft.com/dashboard/) och leta upp den tillgängliga prislistan.

- Lär dig mer [om att köpa Azure-planen](purchase-azure-plan.md)

- Se [prislistan för den nya handelsupplevelsen i CSP](azure-plan-price-list.md)
