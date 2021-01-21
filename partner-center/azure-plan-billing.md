---
title: Fakturering av Azure-plan – faktura & rekognoseringar-filer
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du får åtkomst till och förstår den faktura och avstämnings fil struktur som är relaterad till faktureringen för Azure-prenumerationen.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: e230cc0d8ff3afea4bf2cc7b55d3847814696af6
ms.sourcegitcommit: f99424919f0d77bbe4f44293d84f9ea1e3317f13
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/21/2021
ms.locfileid: "98658441"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Ny handelsupplevelse i CSP – Azure-fakturering 

**Lämpliga roller**

- Administratörs agent
- Faktureringsadministratör
- Global administratör

Den här artikeln förklarar hur du får åtkomst till och förstår strukturen på fakturan och avstämnings filen som är relaterad till faktureringen för Azure-prenumerationen. Faktureringen enligt Azure-planen är en förenklad fakturerings upplevelse med ett justerat fakturerings datum och en månads-baserad fakturerings period.

## <a name="summary-of-billing-essentials"></a>Sammanfattning av fakturerings grunderna

- **Faktura datum**: faktura-och avstämnings fil kommer att finnas i Partner Center Dashboard/API med 8 (midnatt UTC).

- **Fakturerings period för faktura**: faktura fakturerings perioden justeras till kalender månaden, till exempel 10/1-10/31, 11/1-11/30.

- **Debitering av service perioder**: avgifterna justeras till kalender månaden. Om den fakturerade partnern till exempel lägger till Azure-tjänster via en Azure-plan på 10/15 och kunden börjar förbrukningen av Azure-tjänster på 10/15, får fakturerad partner faktura-rekognoseringar på 11/8 för kund förbrukning för service perioden 10/15-10/31. Nästa månads faktura som ska genereras på 12/8 innehåller alla avgifter för service perioden 11/1-11/31.

- **Faktura betalnings villkor**: net 60 dagar.

- **Faktura valuta**: partner kommer fortsätta att faktureras i kundens country's-tilldelade valuta. Om den fakturerade partnern till exempel är i Irland med kunder i Storbritannien, Norge och Tyskland får den fakturerade partnern ett GBP, NOK och faktura/rekognoseringar EUR.

- **Partner incitament**: betalda 45 dagar från slutet av faktura månaden.

## <a name="access-your-invoices-and-reconciliation-files"></a>Få åtkomst till dina fakturor och avstämnings filer

Den globala administratörs-eller fakturerings administratören för ditt företag får ett e-postmeddelande när en faktura är klar att visa.

För att få åtkomst till fakturan och avstämnings filen:

1. Logga in i Partnercenter och gå till [instrumentpanelen](https://partner.microsoft.com/dashboard/).

2. Från menyn Partner Center väljer du **fakturering**.

3. Välj fliken för den **återkommande** **tiden** och den valuta som du är intresse rad av.

   :::image type="content" source="images/azure/billing3.png" alt-text="fakturerings":::

4. Välj **faktura** eller **avstämnings fil**.  

   Om du vill visa historiska fakturor och rekognoseringar-filer expanderar du raden för fakturerings historiken nedan.

## <a name="understanding-usage-data"></a>Förstå användnings data 

1. Azure-prenumeration är rot-eller toppnivå behållaren för användning. All användning är bunden tillbaka till en enda Azure-plan.

2. Inom en plan kommer det att finnas en eller flera Azure-prenumerationer. Dessa är behållare som används för resurs hantering och distribution. 

3. I en prenumeration lägger resurs grupper till i grupp resurser. Varje resurs distribueras till en resurs grupp. 

4. Exempel på resurser är virtuella datorer och lagrings konton. 

5. Antal resurs utsändare: mätare är mätningar av förbrukningen av en resurs och en resurs kan generera användning för flera mätare. Mätare identifieras av ett ProductId-, SKUId-och AvailabilityId. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hierarki för resurs grupper för prenumerationer och mätning

**Azure-konto (klient organisation)**

- Prenumeration A
    - ResourceGroup 1
        - Virtuell dator (resurs)
            - Beräknings mätare
        - Virtuellt nätverk (resurs)
            - Ingen fakturerings mätare

    - ResourceGroup 2
        - Virtuell dator (resurs)
            - Dator mätare
        - Premium SSD-hanterad disk (resurs)
            - Lagrings kapacitets mätare
            - Lagrings åtgärds mätare

- Prenumeration B-ResourceGroup 1 – Azure SQL (resurs)-DTU-mätare-VPN Gateway (resurs) – VPN gateway-mätare

    - ResourceGroup 2
        - Virtual Network gränssnitt (resurs)
            - Ingen fakturerings mätare

## <a name="read-the-invoice"></a>Läs fakturan

1. Fakturan kommer att vara tillgänglig senast den åttonde dagen i varje månad.

2. Partner har 60 dagar på sig att betala.

3. Fakturerings perioden kommer att avse en viss kalender månad, till exempel 10/1-10/31.

4. Avgifterna är netto av justeringar (beloppet är netto av "partner intjänad kredit för tjänster som hanteras").

5. Granska fakturan rekognoseringar-filen och den dagliga, beräknade användnings filen för ytterligare fakturerings information.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Voice":::

## <a name="read-the-invoice-reconciliation-file"></a>Läs faktura avstämnings filen

1. Varje kombination av Azure-plan och-mätare kan ha upp till två fakturerings rader i rekognoseringar-filen.

2. Om mätaren är kvalificerad för någon typ av rabatt eller kredit (till exempel rabatterade rabatter eller partner intjänade kredit för tjänster som hanteras) under hela kalender månaden, kommer rekognoseringar-filen bara att innehålla en fakturerings rad. Kolumnen **PriceAdjusmentDescription** kommer att referera till rabatten eller den intjänade krediten.

3. Om det inte finns några resurser för en viss mätare som är kvalificerad för rabatt eller partner intjänad kredit, kommer rekognoseringar-filen bara innehålla en fakturerings rad och det effektiva enhets priset blir åter försäljnings priset (vilket är enhets priset).

4. Om mätaren eller eventuella resurser som avger denna mätare, kvalificerat för **partner intjänad kredit för tjänster som hanteras** i en del av månaden, innehåller rekognoseringar-filen två fakturerings rader. En rad representerar de dagar som mätaren kvalificeras och den andra raden visar de dagar som mätaren inte kvalificerade sig.

## <a name="read-the-daily-usage-file"></a>Läs den dagliga användnings filen

- Prenumerations mätare enligt en Azure-plan klassificeras och ackumuleras per dag.

- **Partner intjänad kredit för tjänster som hanteras** bestäms och tillämpas dagligen.

- Varje prenumerations mätare har en rad för varje dag i månaden där förbrukningen pågick.

- I exemplet nedan:

  - Mätar kvalificerare för **partner intjänade krediter för tjänster som hanteras** från 7/1-7/3 (Observera att det effektiva enhets priset är i detalj handels pris minus partner intjänande

  - Mätaren var inte berättigad till **partner intjänad kredit för tjänster som hanteras** från 7/4-7/7 (Observera att det effektiva enhets priset är försäljnings pris).

  - Mätning som är kvalificerad för **partner intjänad kredit för tjänster som hanteras** från 7/8-7/31 (Observera att det effektiva enhets priset är åter försäljnings pris minus partner intjänad kredit)

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a>Faktura i kund valuta

Azure-tjänster via en Azure-prenumeration priss ätts i USD och faktureras i kund landets tilldelade valuta. Om fakturerings valutan är icke-USD visas den utländska växelkursen (FX) som används på den sista sidan i fakturan. FX-priser fastställs varje månad och tillämpas på följande faktura. En fullständig lista över lands valutor finns i den [nya Commerces tillgänglighet för land och kund valuta mat ris](https://go.microsoft.com/fwlink/?linkid=2112354).

Microsoft följer Londons aktie kurs för konvertering. Vi använder växelkursen, som är lika med den växelkurs som inhämtats den senaste sekunden i månaden för den senaste arbets dagen i månaden för Londons fondbörs. FX-priserna kommer att uppdateras och vara tillgängliga på dagen före den första av den månad som de gäller.

## <a name="azure-reservations"></a>Azure-reservationer


Om du köper [Azure-reservationer](azure-reservations.md) via en Azure-prenumeration kan du välja antingen en gång eller månatlig fakturering.


## <a name="azure-spending"></a>Utgift i Azure

Den befintliga Azure-utgifts upplevelsen uppdateras för att stödja den nya faktureringen av Azure-plan i Partner Center. Detta gör att partner kan:

- Visa, hantera och ta emot aviseringar för budget uppsättning på en kund nivå 

- Visa totala uppskattade utgifter i en Azure-plan (uppdelad efter resurs och mätar nivå)

Eftersom fakturerings modellen för Azure-tjänster via en Azure-plan är efter löne förbrukning, för att undvika en större faktura än förväntat, kan partner tillämpa en månads budget och spåra procent andelen av användningen. En budget kan tillämpas på en kund eller flera kunder på en och samma tidpunkt. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Utgift i Azure":::

## <a name="next-steps"></a>Nästa steg

- Se hur partnern för intjänad kredit (PEC) beräknas. Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard/) och leta upp pris listan som är tillgänglig.

- Lär dig mer om [att köpa Azure-prenumerationen](purchase-azure-plan.md)

- Se [pris listan för den nya Commerce-upplevelsen i CSP](azure-plan-price-list.md)
