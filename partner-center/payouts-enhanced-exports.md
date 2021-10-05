---
title: Sidan Exportera data för utbetalning
description: Förklarar hur du använder den förbättrade exportdatasidan för att generera anpassade transaktionshistorikrapporter
author: Satinder37
ms.author: sabajaj
ms.topic: how-to
ms.date: 10/04/2021
ms.custom: template-how-to
ms.openlocfilehash: 9ac19a8ea42020b4ec2543d9f4ef197eb95e3a61
ms.sourcegitcommit: cf8c78e0c8831371432007d5ab05f934f15a77b5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/05/2021
ms.locfileid: "129528671"
---
# <a name="payouts-export-data-page"></a>Sidan Exportera data för utbetalning
**Lämpliga roller:** Incitamentsadministratörsroller | Incitamentsanvändare

I den här artikeln beskrivs förbättringar av dataexportupplevelsen för **utbetalning i** Partnercenter. Den här guidade upplevelsen innehåller nya standardmallar för att exportera dina transaktionshistorikrapporter. Den har också en dynamisk funktion som gör att du kan skapa egna anpassade mallar för dina transaktionshistorikrapporter.

## <a name="access-the-export-data-page"></a>Åtkomst till exportdatasidan
1.  Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/home).
2.  Välj **Utbetalningar** och välj sedan **Incitamentexport** eller **Transaktionshistorik** på menyn.

> [!Note] 
> Du får åtkomst till den här sidan om du är [incitamentadministratör eller incitamentsanvändare.](/payout-statement#roles-and-permissionsData) Vad du ser beror på vilka kombinationer av program och Microsoft Partner Network (MPN) som du har åtkomst till (liknar **transaktionshistorik** och **betalningssidor).**

## <a name="export-your-data"></a>Exportera dina data
1.   Välj den typ av data som du vill exportera. 
      - Om du vill visa en transaktionshistorikrapport **väljer du Information om intjäning, transaktion och betalningsstatus.**  Observera att **information om intjäning, transaktion och betalningsstatus (tillväxtreglage)** inte gäller för kommersiella marknadsplatser. 
      - Välj Betalningsinformation för **en betalningsrapport.**
   :::image type="content" source="images/payouts/type-of-data.png" lightbox="images/payouts/type-of-data.png" alt-text="Skärmbild som visar typ av dataval.":::

2.   Välj en rapportmalltyp.

      :::image type="content" source="images/payouts/report-template-type.png" lightbox="images/payouts/report-template-type.png" alt-text="Skärmbild som visar val av rapportmalltyp.":::

      Ditt val för steg 1 avgör mallalternativen för steg 2. Om du till exempel väljer **Intjäning, transaktion, betalningsstatusinformation** i steg 1 visas fyra olika mallalternativ:
      - **Standardtransaktionshistorik:** Den här rapporten visar alla möjliga attribut som är tillgängliga i rapporten för alla program (incitament, kommersiella marknadsplatser och konsumentmarknads marknadsplatser). Det här var nedladdningsmallen som var tillgänglig före oktober 2021.
      - **Standardmarknad:** Den här rapporten visar alla attribut som krävs för MPN-medlemmar som har registrerats i program på den kommersiella marknadsplatsen, till exempel Azure Marketplace. 
      - **Standardarkiv:** Den här rapporten visar alla attribut som krävs för MPN-medlemmar som har registrerats i konsumentarkivet, till exempel Microsoft Store, Minecraft och MS Flight Simulator. 
      - **Anpassad transaktionshistorik:** Med den här rapporten kan du anpassa din transaktionshistorikrapport.

      Om du **väljer Information om intjäning, transaktion** och betalningsstatus i steg 1 kan du välja mallen Transaktionssammanfattning i steg 2.  Om du **väljer Betalningsinformation** i steg 1 visas en "Betalningar"-mall i steg 2. Om du väljer **AGI-intäktsinformation** i steg 1 kan du välja mellan **Programintäkter** eller **Kund** lägger till mallar i steg 2.

3. Välj ett rapportfilformat.
   
      :::image type="content" source="images/payouts/report-file-format.png" lightbox="images/payouts/report-file-format.png" alt-text="Skärmbild som visar val av rapportfilformat.":::

4.   Välj din tidsperiod och tillämpa andra filter och välj sedan Ladda **ned data.**
   
      :::image type="content" source="images/payouts/time-period-filters.png" lightbox="images/payouts/time-period-filters.png" alt-text="Skärmbild som visar rapporttidsval och filteralternativ.":::

> [!Note] 
> Du kan exportera data och hantera begäranden från tabellen **Hämtningsbegäranden.**

## <a name="create-your-customized-transaction-history-report"></a>Skapa din anpassade transaktionshistorikrapport

Anpassa avstämningsrapporten för transaktionshistorik så att den passar dina behov. Du kan skapa och hantera upp till fem rapportmallar. 

1.  Välj **+ Anpassad transaktionshistorik för** att konfigurera en ny avstämningsmall. 
   
      :::image type="content" source="images/payouts/custom-trans-history.png" lightbox="images/payouts/custom-trans-history.png" alt-text="Skärmbild som visar konfiguration av anpassad transaktionshistorik.":::


2.   Ange ett mallnamn och en kort beskrivning och välj **sedan Nästa.**
   
      :::image type="content" source="images/payouts/template-name.png" lightbox="images/payouts/template-name.png" alt-text="Skärmbild som visar nya fält för anpassade avstämningsmallar.":::


3.  Välj de datakolumner som du vill inkludera och granska de standardkolumner som redan visas i rapporten. Välj **Nästa**.
   
     :::image type="content" source="images/payouts/data-selection.png" lightbox="images/payouts/data-selection.png" alt-text="Skärmbild som visar nya datavalsalternativ för anpassade avstämningsmallar.":::

4.  Granska mallinformationen och dataurval, gör ändringar om det behövs och välj sedan **Skapa anpassad mall.**
   
      :::image type="content" source="images/payouts/new-custom-template.png" lightbox="images/payouts/new-custom-template.png" alt-text="Skärmbild som visar bekräftelseskärmen för den nya anpassade avstämningsmallen.":::

5.  Välj **Ladda** ned på nästa skärm för att exportera dina data. Du kan också lägga till, redigera, ladda ned eller ta bort andra mallar från den här skärmen.
   
      :::image type="content" source="images/payouts/download-manage-templates.png" lightbox="images/payouts/download-manage-templates.png" alt-text="Skärmbild som visar alternativ för att hantera mallar och ladda ned data.":::

## <a name="next-steps"></a>Nästa steg
- [Översikt över utbetalning](non-payment-fraud-misuse.md)
- [Intäktssammanfattning](revenue-summary.md)
- [Utbetalningsinstruktioner](payout-statement.md)
- [Vanliga frågor om utbetalning och skatter](payout-faq.yml)
