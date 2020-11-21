---
title: Privata erbjudanden i Azure Marketplace
description: Lär dig om privata erbjudanden i Azure Marketplace.
ms.prod: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 055151f0420d642d591554a829dc21b69df84ebd
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007644"
---
# <a name="private-offers-in-azure-marketplace"></a>Privata erbjudanden i Azure Marketplace

Privata erbjudanden ger utgivare anpassade planer för vissa kunder. Det här alternativet stöds för närvarande endast i Azure Marketplace-miljön i Azure Portal. Privata erbjudanden är bara tillgängliga för avgiftsbelagda erbjudanden som kan köpas och installeras direkt från Azure Portal. Det går inte att skapa privata erbjudanden för konsult tjänster, alla tjänster som har **kontakt mig** som en samtal till åtgärd eller en kostnads fri tjänst, oavsett om den kan installeras från portalen eller inte.

## <a name="find-private-offers-in-the-azure-portal"></a>Hitta privata erbjudanden i Azure Portal

När en partner publicerar ett privat erbjudande, är det bara synligt för berättigade användare i **Marketplace** -avsnittet i Azure Portal. Dessa användare definieras av prenumerations-ID eller klient-ID, beroende på typen av erbjudande. Om du är berättigad till privata erbjudanden finns det två sätt att hitta dem i portalen.

> [!NOTE]
> Privata erbjudanden är för närvarande inte sökbara eller filtrerings bara (efter kategori) i Azure Portal.

I Azure Portal väljer du **+ skapa en resurs** eller söker efter "Marketplace" för att gå till **Marketplace** -sidan. Om du är berättigad till privata erbjudanden visas banderollen för **privata erbjudanden** överst på sidan. Välj **Visa privata erbjudanden** för att gå till din privata erbjudande sida.

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="Den banderoll som visas när du har privata erbjudanden tillgängliga.":::

Alternativt kan du även Rulla längst ned på sidan produkt galleri och visa en delmängd av dina privata erbjudanden om du ser annonsen för privata erbjudanden. Välj länken om du vill **Visa mer** för att gå till din privata erbjudande sida.

:::image type="content" source="media/private-offers/see-more-link.png" alt-text="Visar privata erbjudanden längst ned på skärmen, tillsammans med länken se mer.":::

## <a name="review-private-plans"></a>Granska privata planer

Ett privat erbjudande är i själva verket en privat plan inom ett erbjudande. Varje erbjudande kan ha flera planer, både offentliga och privata, men privata planer visas under en separat lista från offentliga planer.

Du kan se tillgängliga privata planer på fliken **planer** som marker ATS med ett **eget privat** märke:

:::image type="content" source="media/private-offers/private-badge.png" alt-text="En sida med planer som marker ATS som privata.":::

Om du har mer än en prenumeration visas alla privata erbjudanden som är tillgängliga för alla dina prenumerationer. När du väljer **skapa** dirigeras du till sidan för att skapa resurser för att börja konfigurera din resurs.

Om du väljer **skapa** och har flera prenumerationer, men inte alla läggs till i den privata planen, kanske din standard prenumeration inte är den prenumeration som är berättigad till det privata erbjudandet. I det här fallet väljer du rätt prenumeration.

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="Länken som visar att det finns fler privata erbjudanden tillgängliga.":::

## <a name="next-steps"></a>Nästa steg

- [Vad är Azure Marketplace?](azure-marketplace-overview.md)
