---
title: Begränsade direkta fakturerings funktioner
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig mer om krav för CSP direkt fakturerings partner och vad du kan göra för att undvika att funktioner begränsas. Ta reda på om dina funktioner har begränsats.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38fe5d03784d0fcf0796545d31e8272f316d2878
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/06/2021
ms.locfileid: "99623991"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Begränsade direkta fakturerings möjligheter och de krav som krävs för CSP Direct-fakturerings partner  

## <a name="overview"></a>Översikt

Direkta faktura partner måste uppfylla de nya [kraven](direct-partner-new-requirements.md) för att finnas kvar i CSP: n för fakturerings program för CSP. I annat fall kommer deras åtkomst till direkta fakturerings möjligheter att bli begränsad och kan utföra vissa uppgifter, till exempel för att göra nya inköp för kunderna.

> [!Note]
> Direkt fakturerings partner som inte uppfyller de nya kraven för CSP: n för fakturerings program för CSP kommer att informeras av Microsoft när deras direkta fakturerings funktioner kommer att begränsas. Detta gäller för alla direkta fakturerings partner, oavsett om de har valt att [övergå från direkt fakturerings partner till indirekta åter försäljare](transition-direct-to-indirect.md) eller inte.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Så här ser du om dina direkta fakturerings funktioner har begränsats

Följ dessa steg för att kontrol lera om åtkomsten från direkt fakturerings partnerns klient organisation till direkta fakturerings funktioner har begränsats.

1. Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard).

2. Gå till **konto inställningar**  ->  **juridisk profil**.

3. Leta efter **Microsoft Cloud lösnings leverantörens status** under **programinformation**.

4. Om programmets status har värdet **begränsat** innebär det att din direkt fakturerings partners klient organisations åtkomst till direkta fakturerings funktioner har begränsats.

## <a name="affected-direct-bill-capabilities"></a>Berörda direkt fakturerings funktioner

Om dina direkta fakturerings funktioner har begränsats kan du inte längre göra nya inköp för dina kunder i Partner Center. Den här begränsningen omfattar:

- Azure-prenumerationer

- Licensbaserade prenumerationer

- Lägg till nya tillägg i befintliga licensbaserade prenumerationer.

- Gör engångs inköp av program varu-och reservations produkter (till exempel program varu prenumerationer, beständig program vara och reserverade instanser av virtuella Azure-datorer).

Du kan inte heller använda [Azure partners delade tjänster-erbjudandet](shared-services.md) under CSP-programmet för att köpa nya Azure-prenumerationer för eget bruk.

Befintliga prenumerationer på direkt fakturering påverkas inte. De förblir giltiga och förnyas automatiskt. Du kommer fortsätta att faktureras direkt av Microsoft tills de har annullerats. Du kan fortfarande hantera befintliga prenumerationer på följande sätt:

- Pausa befintliga prenumerationer

- Justera licens antalet för befintliga licensbaserade prenumerationer

- Justera licens antalet för befintliga tillägg i en prenumeration. 
 
    >[!Note] 
    >Du kan inte lägga till nya tillägg i befintliga prenumerationer eftersom det behandlas som ett nytt köp.

- Distribuera nya Azure-resurser och hantera befintliga Azure-resurser under befintliga Azure-prenumerationer. Detta inkluderar resurser som är tillgängliga via Azure Marketplace-och Visual Studio-prenumerationer.

Förutom nya köp kan du inte komma åt följande direkta fakturerings funktioner i Partner Center:

- Du kan inte skapa nya kund klienter. Alternativet **Skapa kund** på sidan **kunder** i Partner Center är inte tillgängligt.

- Du kan inte skapa inbjudan till kund förfrågan om direkt åter försäljarens relation. Alternativet **begär en åter försäljare-relation** på sidan **kunder** i Partner Center är inte tillgängligt.

    >[!NOTE]
    >Som en del av över gången från direkt fakturerings partner till indirekt åter försäljare, om du redan har registrerat din leverantör av direkt fakturerings partner som indirekt åter försäljare, kan du generera inbjudan till kund förfrågan om indirekt åter försäljarens relation i stället.

- Du kan inte skapa en ny Sand Box klient. Varje leverantör av direkt fakturerings partner kan skapa en sand Box klient för syftet med direkt fakturerings-API-integrering. Om du inte har skapat någon tidigare, kan du inte göra det när du har fått en begränsad kapacitet för fakturerings partner.  

## <a name="next-steps"></a>Nästa steg

- [Ytterligare information om att bli en indirekt åter försäljare](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [CSP Direct-partner nya krav](direct-partner-new-requirements.md)
