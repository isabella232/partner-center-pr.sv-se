---
title: Fakturering – licensbaserade SaaS-transaktioner
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Lär dig mer om vanliga faktureringsscenarier i Partnercenter för licensbaserade SaaS-transaktioner (programvara som en tjänst).
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9568a014de926682dd89dd9d06d1c6ca5b98ac71
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960066"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Vanliga faktureringsscenarier för licensbaserade SaaS-transaktioner i Partnercenter

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Supportagent | Försäljningsagent


Dessa exempel [på vanliga faktureringsscenarier](common-billing-scenarios.md) gäller för licensbaserade SaaS-prenumerationer (programvara som en tjänst) i Partnercenter.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Konvertera en kostnadsfri Utvärderingsversion av SaaS-prenumeration till en betald prenumeration

Det här scenariot beskriver fakturering för förnyelse av en licensbaserad kostnadsfri utvärderingsversion av SaaS-prenumeration. Förnyelsen konverterar den kostnadsfria utvärderingsversionen till en betald prenumeration i slutet av den kostnadsfria utvärderingsperioden.

I det här exemplet köpte du en kostnadsfri utvärderingsversion av en licensbaserad SaaS-prenumeration (programvara som en tjänst) den 10 juni. Den här kostnadsfria utvärderingsversionen förnyas automatiskt som en betald prenumeration när den kostnadsfria utvärderingsperioden upphör.

Rekognoseringsfilerna inkluderar följande avgifter:

| Inköpsdatum | Startdatum för avgift | Slutdatum för avgift | Enhetspris | Enhetskvantitet | Totalmängd | Kostnadstyp | Prenumerationsbeskrivning |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 1 | 0 USD | Ny | Kostnadsfri utvärderingsversion |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | 2 USD | 1 | 2 USD | Förnya | Betald prenumeration |

## <a name="cancel-a-free-trial-saas-subscription"></a>Avbryta en kostnadsfri utvärderingsprenumeration på SaaS

> [!TIP]
> Du kan avbryta en licensbaserad kostnadsfri utvärderingsversion av SaaS när som helst, även under den kostnadsfria utvärderingsperioden.

I det här scenariot köpte du en licensbaserad kostnadsfri utvärderingsprenumeration på SaaS den 1 juli och avbröt den sedan direkt i Partnercenter.

Rekognoseringsfilen innehåller följande avgifter:

| Inköpsdatum | Startdatum för avgift | Slutdatum för avgift | Enhetspris | Enhetskvantitet | Totalmängd | Kostnadstyp | Prenumerationsbeskrivning |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Ny | Kostnadsfri utvärderingsversion |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Avbryt | Kostnadsfri utvärderingsversion |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Konvertera en anpassad SaaS-mätarprenumeration till en annan SKU

Det här scenariot beskriver hur du konverterar en anpassad SaaS-mätarprenumeration från en lagerhållningsenhet (SKU) till en annan SKU för samma produkt, på samma datum.

I det här scenariot köpte du en SKU (Silver) under en produkt och konverterade den till en annan tillgänglig SKU (brons) under den här produkten samma datum.

Rekognoseringsfilen innehåller följande avgifter:

| Inköpsdatum | SKU | Startdatum för avgift | Slutdatum för avgift | Enhetspris | Enhetskvantitet | Totalmängd | Kostnadstyp | Prenumerationsbeskrivning |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | 20 USD | 1 | 20 USD | Ny | Anpassad SaaS-mätarprenumeration |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | 20 USD | 1 | -$20 | Konvertera | Fakturerad omfakturering för saaS-prenumeration med anpassad mätare |
| 06/10/2019 | Brons | 06/10/2019 | 06/10/2019 | 10 USD | 1 | 10 USD | Konvertera | Anpassad SaaS-mätare-prenumeration |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Köpa och avbryta en SaaS-prenumeration på kundmätare samma datum

I det här scenariot beskrivs faktureringen för en SaaS-prenumeration med kundmätare som du har köpt och avbrutit Azure Portal samma datum.

I det här scenariot har du köpt en anpassad SaaS-mätare-prenumeration på Azure Portal. Sedan avbröt du prenumerationen på samma datum.

| Inköpsdatum | SKU | Startdatum för avgift | Slutdatum för avgift | Enhetspris | Enhetskvantitet | Totalmängd | Kostnadstyp | Prenumerationsbeskrivning |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Brons | 06/10/2019 | 06/10/2019 | 10 USD | 1 | 10 USD | Ny | Anpassad SaaS-mätare-prenumeration |
| 06/10/2019 | Brons | 06/10/2019 | 06/10/2019 | 10 USD | 1 | -$10 | CancelImmediate | Anpassad SaaS-mätare-prenumeration |
