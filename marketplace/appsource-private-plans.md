---
title: Privata planer i Microsoft AppSource
description: Konfigurera privata planer i Microsoft AppSource (Azure Marketplace).
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123936932"
---
# <a name="private-plans-in-microsoft-appsource"></a>Privata planer i Microsoft AppSource

Privata planer är hur utgivare tillhandahåller anpassade planer till specifika kunder. Det här alternativet är nu tillgängligt i Microsoft AppSource. Privata planer kan säljas på AppSource för SaaS-erbjudanden (programvara som en tjänst) med anropet Get **it now** call-to-action (Hämta det nu).

## <a name="ask-your-isv-for-a-private-plan"></a>Be din ISV om en privat plan

För att en privat plan ska vara tillgänglig för dig i AppSource måste du kontakta ISV:en direkt och förhandla ett anpassat pris och tekniska specifikationer. När villkoren i den privata planen har godkänts skapar ISV:n en plan för dig och tilldelar den till din organisations klientorganisations-ID, som du måste ange.

### <a name="finding-your-tenant-id"></a>Hitta ditt klientorganisations-ID

1. I AppSource, i det övre högra hörnet, väljer du ikonen för din kontoprofil och sedan **Visa klientorganisation.**
2. Kopiera klientorganisations-ID:t och ange det till ISV:n.

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Visar hur du hittar ditt klientorganisations-ID.":::

## <a name="find-a-private-plan-in-appsource"></a>Hitta en privat plan i AppSource

Det kan ta upp till 48 timmar efter att ISV:en har publicerat den nya privata planen innan du ser den i AppSource. Om du vill hitta privata planer som är associerade med ditt **klientorganisations-ID** väljer du Privata planer (låsikonen) längst upp till höger i AppSource.

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="Visar låsikonen (hänglås) i det övre verktygsfältet.":::

Om du inte är inloggad uppmanas du att göra det i ett meddelande. Du kan sedan köpa de privata planer som är associerade med ditt klientorganisations-ID **på fliken Planer +** prissättning.

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Visar privata erbjudanden på fliken plan och prissättning.":::

Om privata planer inte är tillgängliga för din klientorganisation visas ett meddelande om att du inte har några privata planer eller erbjudanden.

## <a name="purchase-a-private-plan"></a>Köpa en privat plan

En ISV kan innehålla en eller flera privata planer i ett erbjudande. Varje erbjudande kan ha både offentliga och privata planer, men privata planer visas under en separat erbjudandelistsida som nås från ikonen privata erbjudanden (hänglås) längst upp till höger på sidan.

Tillgängliga privata planer visas på **fliken Planer +** priser. Privata planer har ett blått märke.

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="Visar märke för det blå privata erbjudandet bredvid privata erbjudanden.":::

Om du vill köpa en vald plan **väljer du Hämta nu** och följer de angivna stegen.

## <a name="next-steps"></a>Nästa steg

- [Vad är Microsoft AppSource?](appsource-overview.md)
