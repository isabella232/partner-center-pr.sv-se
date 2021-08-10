---
title: Begränsade funktioner för direktfakturering
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Lär dig Molnlösningsleverantör partnerkrav för direktfakturering (CSP) och vad du kan göra för att undvika att funktioner begränsas. Ta reda på om dina funktioner har begränsats.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f3027ec26586e7d96a5d9ac3d6db8e2297c61db194da1f00353091fc13e48915
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115682682"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Begränsade funktioner för direktfakturering och de krav som krävs för CSP-partner med direktfakturering

**Lämpliga roller:** Global administratör

## <a name="overview"></a>Översikt

Direktfaktureringspartner måste uppfylla [de nya](direct-partner-new-requirements.md) kraven för att finnas kvar Molnlösningsleverantör CSP-partnerprogrammet (Direct Bill). Annars kommer deras åtkomst till direktfaktureringsfunktionerna så småningom att begränsas och kan längre utföra specifika uppgifter, till exempel att göra nya inköp för sina kunder.

> [!Note]
> Direktfaktureringspartner som inte uppfyller de nya kraven för CSP-partnerprogrammet för direktfakturering informeras av Microsoft när deras funktioner för direktfakturering kommer att begränsas. Detta gäller för alla direktfaktureringspartner, oavsett om de har valt en övergång från [direktfaktureringspartner till indirekta återförsäljare](transition-direct-to-indirect.md) eller inte.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Så här ser du om dina direktfaktureringsfunktioner har begränsats

Följ dessa steg för att bekräfta om åtkomsten från partnerklientorganisationen för direktfakturering till direktfakturering har begränsats.

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).

2. Gå till **Kontoinställningar**  >  **Juridisk profil**.

3. Under **Programinfo** letar du upp **Leverantör av Microsoft-molnlösningar status**.

4. Om programstatusen har värdet **begränsad** innebär det att direktfaktureringspartnerns åtkomst till direktfaktureringsfunktioner har begränsats.

## <a name="affected-direct-bill-capabilities"></a>Funktioner för direktfakturering som påverkas

Om dina direktfaktureringsfunktioner har begränsats kan du inte längre göra nya inköp för dina kunder i Partnercenter. Den här begränsningen omfattar:

- Azure-prenumerationer

- Licensbaserade prenumerationer

- Lägg till nya tillägg till befintliga licensbaserade prenumerationer.

- Gör ett köp av programvara och reservationsprodukter (till exempel programvaruprenumerationer, permanent programvara och instanser av reserverade virtuella Azure-datorer).

Du kan inte heller använda [erbjudandet om delade Azure-partnertjänster](shared-services.md) under CSP-programmet för att köpa nya Azure-prenumerationer för eget bruk.

Befintliga prenumerationer på direktfakturering påverkas inte. De förblir giltiga och är automatiskt nya. Du fortsätter att debiteras direkt av Microsoft tills de avbryts. Du kan fortfarande hantera befintliga prenumerationer på följande sätt:

- Pausa befintliga prenumerationer

- Justera licensantalet för befintliga licensbaserade prenumerationer

- Justera antalet licenser för befintliga tillägg till en prenumeration. 

    >[!Note]
    >Du kan inte lägga till nya tillägg till befintliga prenumerationer eftersom det behandlas som ett nytt köp.

- Distribuera nya Azure-resurser och hantera befintliga Azure-resurser under befintliga Azure-prenumerationer. Detta omfattar resurser som är tillgängliga via Azure Marketplace och Visual Studio prenumerationer.

Förutom nya köp kan du inte komma åt följande funktioner för direktfakturering i Partnercenter:

- Du kan inte skapa nya kundklienter. Alternativet **Skapa kund** under sidan **Kunder** i Partnercenter är inte tillgängligt.

- Du kan inte skapa en inbjudan till en kund som begär en direkt återförsäljarrelation. Alternativet **Begär en återförsäljarrelation** under **sidan** Kunder i Partnercenter är inte tillgängligt.

    >[!NOTE]
    >Som en del av övergången från direktfaktureringspartner till indirekt återförsäljare kan du, om du redan har registrerat din partnerklient för direktfakturering som indirekt återförsäljare, generera en inbjudan till kunden som begär en indirekt återförsäljarrelation i stället.

- Du kan inte skapa en ny sandbox-klientorganisation. Varje partnerklient för direktfakturering kan skapa en sandbox-klientorganisation för API-integrering med direktfakturering. Om du inte har skapat någon tidigare kan du inte göra det när din partnerfunktion för direktfakturering har begränsats.  

## <a name="next-steps"></a>Nästa steg

- [Ytterligare information om hur du blir en indirekt återförsäljare](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Nya krav för CSP-direktpartner](direct-partner-new-requirements.md)
