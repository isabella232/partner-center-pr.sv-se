---
title: Privata planer i Azure Marketplace
description: Lär dig mer om privata planer i Azure Marketplace.
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 08/27/2021
ms.openlocfilehash: d8c55ce8f6a0c5da3bf2f02c899196e8fd6fd2e0
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247014"
---
# <a name="private-plans-in-azure-marketplace"></a>Privata planer i Azure Marketplace

Privata planer är hur utgivare tillhandahåller anpassade planer till specifika kunder. Privata abonnemang är endast tillgängliga för betalda produkter som kan köpas och installeras direkt från Azure Portal. Utgivare kan inte skapa privata planer för  konsulttjänster, tjänster som har Kontakta mig som en call-to-action eller någon kostnadsfri tjänst, oavsett om de kan installeras från portalen eller inte.

## <a name="find-private-plans-in-the-azure-portal"></a>Hitta privata planer i Azure Portal

När en partner publicerar en privat plan visas den endast för berättigade användare i **Avsnittet Marketplace** i Azure Portal. Dessa användare definieras av prenumerations-ID eller klientorganisations-ID, beroende på erbjudandetyp. Om du är berättigad till privata planer finns det två sätt att hitta dem i portalen.

> [!NOTE]
> Privata planer är sökbara men inte filtrerbara (efter kategori) i Azure Portal.

I Azure Portal väljer du **+ Skapa en resurs eller** söker efter "marketplace" för att gå till **Marketplace-sidan.** Om du är berättigad till privata abonnemang visas banderollen You **have private products available** (Du har privata produkter tillgängliga) överst på sidan. Välj **Visa privata produkter för** att gå till sidan med dina privata abonnemang.

:::image type="content" source="media/private-offers/private-products-banner.png" lightbox="media/private-offers/private-products-banner.png" alt-text="Banderollen som visas när du har privata produkter tillgängliga.":::

## <a name="review-private-plans"></a>Granska privata planer

En privat plan ingår i flera planer i en produkt. Varje produkt kan ha flera planer, både offentliga och privata, men privata planer visas under en separat lista från offentliga planer.

Du kan se tillgängliga privata planer under fliken **Planer,** markerat med ett privat **märke:**

:::image type="content" source="media/private-offers/private-badge.png" alt-text="En sida med planer markerade som Privata.":::

Om du har fler än en prenumeration visas alla privata abonnemang som är tillgängliga för alla dina prenumerationer. När du väljer **Skapa** dirigeras du till sidan för resursskapande för att börja konfigurera resursen.

Om du väljer **Skapa** och har flera prenumerationer, men inte alla läggs till i den privata planen, kanske din standardprenumeration inte är den prenumeration som är berättigad för den här privata planen. I det här fallet väljer du rätt prenumeration.

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="Länken visar att det finns fler tillgängliga privata planer.":::

## <a name="next-steps"></a>Nästa steg

- [Vad är Azure Marketplace?](azure-marketplace-overview.md)
