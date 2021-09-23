---
title: Sälja lokal programvara via CSP
ms.topic: how-to
ms.date: 03/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Lär dig hur partner i CSP-programmet kan köpa, hantera, sälja och avbryta lokala programvaruprenumerationer för kunders räkning i Partnercenter.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f58f120d376b98f9fa054f0bec87f324874ce0bb
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/23/2021
ms.locfileid: "128322092"
---
# <a name="sell-on-premises-software-through-the-cloud-solution-provider-csp-program"></a>Sälja lokal programvara via programmet Molnlösningsleverantör (CSP)

**Lämpliga roller:** Administratörsagent | Global administratör

Lokal programvara i CSP stöder en smidig övergång till molnet genom att lokala program introduceras i ett molnfokuserat program. Det här nya erbjudandet hjälper till att ta den mervärdespartnern till varje inköpsscenario eftersom de tillhandahåller en enda plattform för att köpa alla Microsoft-produkter. Som CSP kan du nu sälja lokal programvara via Partnercenter utöver Open, EA och andra program som används för närvarande.  
 
Samtidigt som vi säkerställer det bästa övergripande kundvärdet med lokala programvarulicensieringsalternativ, har vi även gjort affärsmodellen så partnervänlig som möjligt. Enkel licensiering av lokal programvara i CSP innebär kostnads förutsägbarhet och en smidig försäljningsprocess åt dig. Den här nya affärsmodellen gör det enkelt att köpa in, hantera och prissätta lokal programvara för dina kunder, så att du kan fokusera på att vinna verksamhet med en utökad portfölj med mervärdeslösningar för IT-hantering.

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a>Köp programvaruprenumerationer för kunders räkning

Om du vill köpa programvaruprenumerationer åt en kund går du till kundens informationssida, väljer Lägg till produkter och följer sedan anvisningarna på skärmen för att skapa och betala för din beställning.

> [!NOTE]
> Mer information finns i den här [guiden för att beställa och uppfylla via Partnercenter.](https://partner.microsoft.com/resources/detail/guide-to-ordering-and-fulfillment-through-partner-center-pdf)

## <a name="activate-and-manage-software-subscriptions"></a>Aktivera och hantera programvaruprenumerationer

När du har köpt din programvara måste du eller dina kunder ladda ned den (partner som använder Partnercenter; kunder som använder Microsoft 365 Admin Center). Gör detta på följande sätt. Det är viktigt att förstå riskerna med att kopiera länkar och ladda ned programvara. Mer information finns i Använda **Partnercenter för att hämta** nedladdning av kundprogramvara och licensnycklar i [partnercentrets guide för nya handelsåtgärder.](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)

> [!NOTE]
> Du måste vara administratörsagent i Partnercenter för att få en länk till nycklar och nedladdningar.

1. Gå till kundens informationssida och välj sedan **Programvara**. Du ser en lista över all programvara som du har köpt för kundens räkning.

2. Välj **produktversion,** **språk**, **bit** och välj **Hämta nycklar och nedladdningar.** 

3. Välj **Hämta nyckel** som visar den 32-siffriga produkten i ett popup-fönster som du kan kopiera och skicka till kunden. 

4. Välj **Ladda ned** för att ladda ned bitarna. 

5. Välj **Kopiera länk** om du vill skicka kunden länken till bithämtningen. 

6. Du kan också **avbryta programvarubeställningen** och få 100 % kredit (om det görs inom 60-dagarsperioden för annulleringsprincipen).

> [!NOTE]
> Endast kunder har åtkomst till att se produktnycklarna och ladda ned information i Microsoft 365 Admin Center (global administratörsroll krävs). Partner måste använda Partnercenter för att se den här informationen.

> [!NOTE]
> CSP-köp aktiveras via en fleraktiveringsnyckel (MAK). nyckelhanteringstjänst (KMS) (KMS)-nycklar tillåts inte, inte ens vid begäran. 

## <a name="move-a-customers-on-premises-license-from-vl-to-csp-with-no-downtime"></a>Flytta en kunds lokala licens från VL till CSP utan avbrottstid

Även KMS nycklar inte är tillgängliga i CSP kan du fortfarande flytta kundens lokala licenser från VL till CSP och förhindra driftstopp på grund av inköpskanalväxeln. KMS distribuerar licenserna till klienterna och de förblir vanligtvis aktiva i 180 dagar innan enheten försöker förnya aktiveringen. Det innebär att enheten redan är aktiverad och körs under en tid innan några problem uppstår. 

Om kunden distribuerar den nya fleraktiveringsaktiveringsaktiveringen under den här tiden, antingen manuellt eller med skript (med hjälp av ), sker `slmgr.vbs` ingen stilleståndstid. Om kunden inte distribuerar den nya fleraktiveringsaktiveringsaktiveringen under den här tiden och försöker förnya licensen senare, kan enheten bli begränsad eller blockerad i vissa funktioner tills den återaktiveras. 

Mer information finns i Aktivera [klienter som kör Windows 10 (Windows 10) – Windows Distribution](/windows/deployment/volume-activation/activate-windows-10-clients-vamt#key-management-service-activation-renewal). Om du behöver hjälp med den här typen av distribution kan du skicka en begäran om teknisk support och [distributionstjänster.](/partner-center/technical-benefits#submit-a-technical-presales-and-deployment-services-request)

## <a name="cancel-a-purchase"></a>Avbryta ett köp

Använd följande procedur för att avbryta ett köp. När annulleringen är klar återkallas programvarunyckeln.

> [!NOTE]
> Du måste vara administratörsagent för att kunna avbryta ett köp. 

1.  Kontrollera att du har följande innan du påbörjar processen: 
    - Kundens klientorganisations-GUID eller domännamn
    - Order-ID eller prenumerations-ID
    - Orsak till återbetalning
    - Begärd mängd

2.  På kundens informationssida väljer du **Programvara**. Du ser en lista över alla program som du har köpt. 

3.  Leta upp den programvara som du vill avbryta och välj **Avbryt.** Sidan **Rapportera ett problem med Partnercenter** öppnas. 

4.  Under **Information** går du till **listan Typ av problem** och väljer **CSP Purchase/Refund (Köp/återbetalning för CSP) för kunders räkning.**

5.  Fyll i fälten **Impact (Effekt)** **och Title (Rubrik).** 

6.  I **fältet Beskrivning** anger du följande: 
    -   Kundens klientorganisations-GUID eller domännamn
    -   Order-ID eller prenumerations-ID
    -   Orsak till återbetalning
    -   Begärd mängd

7.  I fältet **Kontakt** anger du ditt namn, din e-postadress och ditt telefonnummer. 

8.  Om du behöver bifoga en fil av någon anledning väljer du Lägg **till filer**. Det här är valfritt. 

9.  När du är klar väljer du **Skicka**.
