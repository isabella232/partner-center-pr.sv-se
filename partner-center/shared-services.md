---
title: Lägg till delade Azure-partner tjänster
description: Använd Azure partners delade tjänster för att köpa Azure-prenumerationer för eget bruk och för att få en enhetlig metod för att köpa, spåra och hantera Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: a59cf0b271a0ccf5fd5a1d8e3e85ff43818a3801
ms.sourcegitcommit: fe867be44de3479607be3309940b904d7ea9fc6e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/06/2021
ms.locfileid: "102247705"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Lägg till delade Azure partner-tjänster så att partner kan köpa Azure-prenumerationer för egen användning

 
**Lämpliga roller**

- Global administratör
- Administratörs agent
- Försäljnings agent

Delade Azure partner-tjänster är en ny erbjudande typ för partner i CSP-programmet och gör det möjligt för partner att köpa Azure-prenumerationer för eget bruk.Det skapar möjligheten för partner att använda en enhetlig metod för att köpa, spåra och hantera Azure förutom möjligheten att konsolidera sin Azure-licens och sälja avtal med Microsoft. Med Azure partners delade tjänster har partner nu samma flexibilitet att använda Azure-prenumerationer i CSP som de gör i Microsoft Enterprise-avtal-och WebDirect-program, öppna scenarier som: skapa utvecklings-och test miljöer, distribuera interna arbets belastningar och värdbaserade delade tjänster eller program med flera klienter.  

## <a name="create-the-shared-services-tenant"></a>Skapa klienten för delade tjänster

1. Gå till **Inställningar**  >  **konto inställningar**  >  **delade tjänster**.

   :::image type="content" source="images/sharedservices2.png" alt-text="Konto inställningar > delade tjänster":::

2. Om du inte redan har en klient för delade tjänster, klickar du på **skapa delade tjänster**.

   :::image type="content" source="images/sharedservices3.png" alt-text="Skapa delade tjänster":::

3. Detta skapar en klient för delade tjänster och köper prenumerationen på delade Azure CSP-tjänster, som ska användas för delade resurser och intern arbets belastning.

   :::image type="content" source="images/sharedservices5.png" alt-text="Skapa klienten och Köp prenumerationen":::

## <a name="about-the-azure--internalshared-services-offer"></a>Om Azure – interna/delade tjänster erbjudandet

- Azure – interna/delade tjänster prenumerationen är en ny Azure-erbjudande typ i CSP som nås via partner Center som partner kan använda för sin egen användning av Azure.

- Prenumerationer på delade Azure partner-tjänster är berättigade och kan användas för att köpa RIs.

- Azure – interna/delade tjänster erbjudandet kan bara tillämpas på den delade tjänstens klient organisation.

- Den primära användningen för Azure – interna/delade tjänster prenumerationen är så att du kan använda Azure i dina egna utvecklings syfte. Den delade klient organisation som du använder för att etablera det här erbjudandet kan inte användas för andra tjänster, till exempel Office 365 eller Dynamics-licenser.

- Du kan avbryta prenumerationen på samma sätt som andra prenumerationer. Gå till **Inställningar**  >  **Visa alla inställningar**  >  **delade tjänster**. Välj Azure – interna/delade tjänster prenumerationen och Avbryt den.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Åtkomst till förbruknings information om Azure partner Shared Services

Du hittar Azure-förbrukningen på din CSP-faktura och i avstämnings filen. Den ingår som en del av Microsoft Azure rads objekt på fakturan. Den detaljerade förbruknings informationen är tillgänglig i avstämnings filen som loggats mot den klient som skapades för erbjudandet.

## <a name="azure-partner-shared-services-pricing"></a>Priser för delade Azure-partner tjänster

Om du vill se den nya pris filen för Azure-partner delade tjänster går du till **försäljnings**  >  **priser och erbjudanden** och väljer den aktuella månadens pris lista. Under de närmaste veckorna frigörs ett särskilt pris-API.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Marketplace-erbjudanden och delade Azure-partner tjänster

Från och med den 1 mars 2019 stöder inte längre Azure partners delade tjänster (APSS) Marketplace-erbjudanden.

|**Marketplace-support**   |**APSS som stöds före den 1 mars 2019**|**Efter den 1 mars 2019**|
|---------------------------|:----------------------------|:-------------------|
|Bring your own license (BYOL) och kostnads fria tjänster   | Ja   | Inga|
|Andra tredje parts Marketplace-erbjudanden   | Inga   |Inga|

Partner som har BYOL eller kostnads fria tjänster som distribueras med APSS påverkas inte. men efter den 1 mars 2019 kommer de inte att kunna köpa nya BYOL eller kostnads fria tjänster.

För att kunna dra nytta av den fullständiga katalogen med Marketplace-erbjudanden (inte bara BYOL och kostnads fria tjänster) rekommenderar vi att CSP-partner distribuerar delade tjänster med hjälp av Web Direct Azure-prenumerationer.  CSP-partner som har distribuerat BYOL från tredje part och kostnads fria tjänster från Marketplace tidigare och som vill fortsätta använda dem och distribuera fler erbjudanden från tredje part uppmanas att migrera APSS-prenumerationen till webb direkt [migrering av befintliga Azure-prenumerationer](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).

Partner, som planerar att fortsätta använda APSS-prenumerationen efter den 1 mars 2019 och vill distribuera nya [BYOL-tjänster](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) från tredje part eller kostnads fria tjänster, kan följa anvisningarna från ISV: er för att distribuera dessa till sina APSS-prenumerationer.

## <a name="next-steps"></a>Nästa steg

- [Sälja programvaruprenumerationer via CSP](csp-software-subscriptions.md)