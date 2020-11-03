---
title: Fakturerings licenser-baserade SaaS transaktioner
ms.topic: article
ms.date: 05/05/2020
description: Lär dig om vanliga fakturerings scenarier i Partner Center för licensierade, SaaS-transaktioner (Software-as-a-Service).
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d63e8345bf127cb91f1812193b1f0311cd569b3
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/14/2020
ms.locfileid: "92531888"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Vanliga fakturerings scenarier för licensbaserade SaaS-transaktioner i Partner Center

**Lämpliga roller**

- Administratörs agent
- Faktureringsadministratör
- Support agent
- Försäljnings agent


Dessa exempel på [vanliga fakturerings scenarier](common-billing-scenarios.md) är tillämpliga för SaaS-prenumerationer (Software as a Service) i Partner Center.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Konvertera en prenumeration för kostnads fri utvärderings SaaS till en betald prenumeration

Det här scenariot beskriver fakturering för förnyelse av en licensbaserade SaaS prenumeration på kostnads fri utvärdering. Förnyelsen konverterar den kostnads fria utvärderings versionen till en betald prenumeration i slutet av den kostnads fria utvärderings perioden.

I det här exemplet har du köpt en kostnads fri utvärderings version av en licens-baserad SaaS (program vara som en tjänst) den 10 juni. Den här kostnads fria utvärderings versionen förnyas automatiskt som en betald prenumeration när den kostnads fria utvärderings perioden är slut.

Rekognoseringar-filerna innehåller följande kostnader:

| Inköps datum | Start datum för debitering | Debiterings slutdatum | Enhetspris | Enhets antal | Totalmängd | Kostnadstyp | Beskrivning av prenumeration |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 1 | 0 USD | Ny | Kostnadsfri utvärderingsversion |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | $2 | 1 | $2 | Förnya | Betald prenumeration |

## <a name="cancel-a-free-trial-saas-subscription"></a>Avbryta en kostnads fri utvärderings version SaaS-prenumeration

> [!TIP]
> Du kan avbryta en licensbaserade SaaS prenumeration när som helst, även under den kostnads fria utvärderings perioden.

I det här scenariot har du köpt en licens fri utvärderings version SaaS-prenumeration den 1 juli och avbröt den omedelbart i Partner Center.

Rekognoseringar-filen innehåller följande kostnader:

| Inköps datum | Start datum för debitering | Debiterings slutdatum | Enhetspris | Enhets antal | Totalmängd | Kostnadstyp | Beskrivning av prenumeration |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Ny | Kostnadsfri utvärderingsversion |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Avbryt | Kostnadsfri utvärderingsversion |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Konvertera den anpassade mätar SaaS-prenumerationen till en annan SKU

I det här scenariot beskrivs hur du konverterar en anpassad mätnings SaaS prenumeration från en lager enhets enhet (SKU) till en annan SKU för samma produkt, på samma datum.

I det här scenariot har du köpt en SKU (Silver) under en produkt och konverterat den till en annan tillgänglig SKU (brons) under den här produkten på samma datum.

Rekognoseringar-filen innehåller följande kostnader:

| Inköps datum | SKU | Start datum för debitering | Debiterings slutdatum | Enhetspris | Enhets antal | Totalmängd | Kostnadstyp | Beskrivning av prenumeration |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | 20 USD | 1 | 20 USD | Ny | Anpassad mätare SaaS-prenumeration |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | 20 USD | 1 | – $20 | Konvertera | Proportionellt Omfakturering för den anpassade mätar SaaS-prenumerationen |
| 06/10/2019 | Brons | 06/10/2019 | 06/10/2019 | 10 USD | 1 | 10 USD | Konvertera | Anpassad mätare SaaS-prenumeration |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Köp och Avbryt en kund mätares SaaS prenumeration på samma datum

I det här scenariot beskrivs faktureringen för en prenumeration på kund mätare SaaS som du har köpt och annullerat genom Azure Portal på samma datum.

I det här scenariot har du köpt en anpassad mätning SaaS-prenumeration på Azure Portal. Sedan avbröt du prenumerationen på samma datum.

| Inköps datum | SKU | Start datum för debitering | Debiterings slutdatum | Enhetspris | Enhets antal | Totalmängd | Kostnadstyp | Beskrivning av prenumeration |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Brons | 06/10/2019 | 06/10/2019 | 10 USD | 1 | 10 USD | Ny | Anpassad mätare SaaS-prenumeration |
| 06/10/2019 | Brons | 06/10/2019 | 06/10/2019 | 10 USD | 1 | – $10 | CancelImmediate | Anpassad mätare SaaS-prenumeration |
