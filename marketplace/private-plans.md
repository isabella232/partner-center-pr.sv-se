---
title: Privata erbjudanden i Azure Marketplace
description: Läs mer om privata erbjudanden i Azure Marketplace.
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 06/03/2021
ms.openlocfilehash: e8a0f0811364de1c012cea7c54bb7b41833d6ce7127d8737c694a3dbc0666ad7
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115688473"
---
# <a name="private-plans-in-azure-marketplace"></a>Privata planer i Azure Marketplace

Privata planer är hur utgivare tillhandahåller anpassade planer till specifika kunder. Privata abonnemang är endast tillgängliga för betalda erbjudanden som kan köpas och installeras direkt från Azure Portal. Utgivare kan inte skapa privata planer för  konsulttjänster, tjänster som har Kontakta mig som en call-to-action eller någon kostnadsfri tjänst, oavsett om de kan installeras från portalen eller inte.

## <a name="find-private-plans-in-the-azure-portal"></a>Hitta privata planer i Azure Portal

När en partner publicerar en privat plan visas den bara för berättigade användare i **Avsnittet Marketplace** i Azure Portal. Dessa användare definieras av prenumerations-ID eller klientorganisations-ID, beroende på erbjudandetyp. Om du är berättigad till privata planer finns det två sätt att hitta dem i portalen.

> [!NOTE]
> Privata planer är sökbara men inte filtrerbara (efter kategori) i Azure Portal.

I den Azure Portal väljer du **+ Skapa en resurs** eller söker efter "marketplace" för att gå till **Marketplace-sidan.** Om du är berättigad till privata planer visas banderollen Du har **tillgängliga privata** planer överst på sidan. Välj **Visa privata erbjudanden + planer för** att gå till sidan för dina privata planer.

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="Banderollen som visas när du har privata planer tillgängliga.":::

## <a name="review-private-plans"></a>Granska privata planer

En privat plan är en del av flera planer i ett erbjudande. Varje erbjudande kan ha flera planer, både offentliga och privata, men privata planer visas under en separat lista från offentliga planer.

Du kan se tillgängliga privata planer under fliken **Planer,** markerade med ett privat **märke:**

:::image type="content" source="media/private-offers/private-badge.png" alt-text="En sida med planer markerade som Privata.":::

Om du har fler än en prenumeration visas alla privata abonnemang som är tillgängliga för alla dina prenumerationer. När du väljer **Skapa** dirigeras du till sidan för resursskapande för att börja konfigurera resursen.

Om du väljer **Skapa** och har flera prenumerationer, men inte alla läggs till i den privata planen, kanske din standardprenumeration inte är den prenumeration som är berättigad för den här privata planen. I det här fallet väljer du rätt prenumeration.

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="Länken som visar att det finns fler privata planer tillgängliga.":::

## <a name="next-steps"></a>Nästa steg

- [Vad är Azure Marketplace?](azure-marketplace-overview.md)
