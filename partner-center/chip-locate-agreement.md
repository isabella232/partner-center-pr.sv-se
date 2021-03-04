---
title: Sök efter antal skriv bord och avgifts nivå
ms.topic: how-to
ms.date: 02/18/2021
description: Lär dig hur du använder kanal incitaments plattform (CHIP) för att hitta information om Skriv bordet och avgifts nivån för ett avtal.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e433b44f158c3e4cefe22027e7f7d3b845991308
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756111"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Leta upp antal skrivbordsenheter och avgiftsnivå för ett avtal

**Lämpliga roller**

- Primär kontakt eller program administratör

Du kan logga in på [Explore.MS](https://www.explore.ms/) för att granska avtalet eller ladda ned en fil som tillhandahåller avtals information för antal skriv bord och avgifts nivåer.

## <a name="to-locate-the-information"></a>För att hitta informationen

### <a name="method-1--explorems"></a>Metod 1 – Explore.ms

1. Öppna [Explore.MS](https://www.explore.ms/) i Internet Explorer. 

>[!Note]
>Du kan inte utföra den här funktionen i Google Chrome eller Microsoft Edge.

2. Logga in med ditt arbets-eller skol konto eller Live-ID.  

3. I fältet **rapporter** väljer du **avtal**.

4. På den resulterande sidan anger du avtals numret i **Sök** fältet och väljer sedan **Välj/ordna kolumner**.

5. I popup-fönstret väljer du **avtal Skriv bords antal** från listan tillgängliga kolumner och väljer sedan högerpilen för att lägga till kolumnen. Välj **OK**.

6. Välj **Sök.**

7. Bläddra igenom resultaten i den resulterande skärmen för att hitta kolumnen **avtal Skriv bords antal** . 

8. Använd Skriv bords antalet för att fastställa avgifts nivån baserat på pris tabellen nedan.  

| Avgifts nivå | Antal skriv bord |
| ------ | :-----------: |
|  A | 0 – 2 399    |
|  B | 2 400 – 5 999    |
|  C | 6 000 – 14 999    |
|  D | 15000 +   |

>[!NOTE]
>Företags incitaments nivåer baseras på Skriv bordet eller antalet användare (det som är högre) i kommersiella och offentliga (PS) registreringar. För registreringar som inte har någon naturlig kopplad Skriv bords-eller användar antal, tillämpar Microsoft ett Skriv bords antal baserat på antalet skriv bord eller antal användare av tillhör ande EA. <br><br>Om det inte finns någon tillhör ande EA, baseras avgifts nivån på pris nivån för registreringen. Pris nivån för affären kan också visas på [www.Explore.MS](https://www.explore.ms/). <br><br>Om det finns flera pooler och/eller pris nivåer för det befintliga EA/EAS, kommer Microsoft att betala incitament till den högsta tilldelade prissättnings-/pool nivån, med nivå A som lägst och nivå D är den högsta.

#### <a name="pool-and-pricing-levels"></a>Pool-och pris nivåer

När du har sökt i avtals numret i explore.ms med hjälp av stegen som beskrivs ovan väljer du avtals numret. Då kommer du till sidan avtals information som visar **avtals Sammanfattning** och **erbjudanden**. Avsnittet med erbjudanden innehåller pris nivåerna.

## <a name="method-2---chip"></a>Metod 2 – CHIP

1. Logga in på kretsen och välj LSP incitament.

2. På sidan **partner betalnings Sammanfattning** väljer du den rapport månad som du vill visa och väljer sedan **beräknings information** i list rutan under **Exportera till Excel**:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Hitta programinformation":::

3. Exporten startar och du kan antingen öppna filen eller spara/Spara som till ett mål.

4. När rapporten är öppen navigerar du till fliken **DetailReport-plattfilsschemagenerator** längst ned till vänster:

:::image type="content" source="images/chip/flatfile.png" alt-text="Flat fil nedladdning":::

Nu kan du söka efter det avtals nummer som du letar efter i kolumn J. och du hittar antalet tilldelade skriv bord i kolumn R, märkta Agreement_DesktopCount. Du kan också bekräfta avgifts nivån för det här avtalet i kolumnens AI-märkta nivå.

## <a name="next-steps"></a>Nästa steg

- [Felsök problem med krets åtkomst](chip-access-trouble.md)
