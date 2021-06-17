---
title: Hitta datorantal och avgiftsnivå
ms.topic: how-to
ms.date: 02/18/2021
description: Lär dig hur du använder CHIP (Channel Incentives Platform) för att hitta information om antal stationära datorer och avgifter för ett avtal.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 288e4ebb224d3ff1b0d4050691b733e678ec29a3
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276950"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Leta upp antal skrivbordsenheter och avgiftsnivå för ett avtal

**Lämpliga roller:** Primär kontakt eller programadministratör

Du kan logga in på [explore.ms](https://www.explore.ms/) granska avtalet eller ladda ned en fil med avtalsinformation för antal skrivbord och avgiftsnivå.

## <a name="to-locate-the-information"></a>Så här hittar du informationen

### <a name="method-1--explorems"></a>Metod 1 – Explore.ms

1. Öppna [explore.ms](https://www.explore.ms/) i Internet Explorer. 

>[!Note]
>Du kan inte utföra den här funktionen i Google Chrome eller Microsoft Edge.

2. Logga in med ditt arbets-/skolkonto eller ditt live-ID.  

3. I fältet **Rapporter** väljer du **Avtal.**

4. På sidan som visas anger du avtalsnumret i **sökfältet** och väljer sedan **Välj/ordna kolumner.**

5. I popup-fönstret väljer du **Antal avtalsdatorer** i listan med tillgängliga kolumner och väljer sedan högerpilen för att lägga till kolumnen. Välj **OK**.

6. Välj **Sök.**

7. På skärmen som visas bläddrar du igenom resultaten för att hitta kolumnen **Antal avtalsdatorer.** 

8. Använd antalet stationära datorer för att fastställa avgiftsnivån baserat på pristabellen nedan.  

| Avgiftsnivå | Antal skrivbord |
| ------ | :-----------: |
|  A | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15,000+   |

>[!NOTE]
>Enterprise-incitamentnivåerna baseras på dator- eller användarantalet (beroende på vilket som är högre) i commercial- och public sector-registreringar (PS). För registreringar utan naturligt associerat antal skrivbord eller användare tillämpar Microsoft ett antal skrivbord baserat på antalet stationära datorer eller antalet användare för tillhörande EA. <br><br>Om det inte finns något tillhörande EA baseras avgiftsnivån på registreringens prisnivå. Prisnivån för avtalet kan också visas på [www.explore.ms](https://www.explore.ms/). <br><br>Om det finns flera pool- och/eller prisnivåer på befintliga EA/EAS betalar Microsoft incitament på den högsta tilldelade prisnivån/poolnivån, där nivå A är lägst och nivå D är högst.

#### <a name="pool-and-pricing-levels"></a>Pool- och prisnivåer

När du har sökt efter avtalsnumret i explore.ms med hjälp av stegen som beskrivs ovan väljer du avtalsnumret. Då kommer du till sidan med avtalsinformation som visar **avtalssammanfattningen** **och erbjudandena**. Avsnittet med erbjudanden innehåller prisnivåerna.

## <a name="method-2---chip"></a>Metod 2 – CHIP

1. Logga in på CHIP och välj LSP Incentives.

2. På sidan **Partnerbetalningssammanfattning** väljer du den rapporteringsmånad som du vill visa och väljer sedan **Beräkningsinformation** i listrutan under **Exportera till Excel:**

:::image type="content" source="images/chip/chiplocate.png" alt-text="Leta upp programinformation.":::

3. Exporten startar och du kan antingen öppna filen eller spara/spara som till ett mål.

4. När rapporten är öppen går du till fliken **DetailReport-FlatFile** längst ned till vänster:

:::image type="content" source="images/chip/flatfile.png" alt-text="Nedladdning av flat fil.":::

Nu kan du söka efter det avtalsnummer som du letar efter i kolumn J. Och du hittar det tilldelade antalet skrivbord i kolumn R, märkt Agreement_DesktopCount. Du kan också bekräfta avgiftsnivån för det här avtalet i kolumnen "AI" med etiketten Nivå.

## <a name="next-steps"></a>Nästa steg

- [Felsöka problem med CHIP-åtkomst](chip-access-trouble.md)
