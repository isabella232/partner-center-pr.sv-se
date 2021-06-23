---
title: Lägga till Azure Partner Shared Services
description: Använd Azure Partner Shared Services att köpa Azure-prenumerationer för eget bruk och för att ha en enhetlig metod för att köpa, spåra och hantera Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 40ba485cecce394dc81632d01f8774859690c522
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551613"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Lägg Azure Partner Shared Services så att partner kan köpa Azure-prenumerationer för eget bruk

**Lämpliga roller:** Globala | Administratörsagent | Försäljningsagent

Azure Partner Shared Services (APSS) är en ny erbjudandetyp för partner i Molnlösningsleverantör-programmet (CSP), vilket gör det möjligt för partner att köpa Azure-prenumerationer för eget bruk.Det skapar möjlighet för partner att använda en enhetlig metod för att köpa, spåra och hantera Azure, utöver möjligheten att konsolidera sina Azure-licensierings- och återförsäljningsavtal med Microsoft. Med APSS har partner nu samma flexibilitet att använda Azure-prenumerationer i CSP som de gör i Microsoft Enterprise-avtal och Web Direct-program, vilket öppnar upp scenarier som: skapa utvecklings- och testmiljöer, distribuera interna arbetsbelastningar och vara värd för delade tjänster eller program för flera innehavare.  

## <a name="create-the-shared-services-tenant"></a>Skapa klientorganisationen för delade tjänster

1. Gå till **Inställningar**  >  **Kontoinställningar**  >  **Delade tjänster.**

   :::image type="content" source="images/sharedservices2.png" alt-text="Kontoinställningar > delade tjänster":::

2. Om du inte redan har en klientorganisation för delade tjänster väljer du **Skapa delade tjänster.**

   :::image type="content" source="images/sharedservices3.png" alt-text="Skapa delade tjänster.":::

3. Detta skapar en klientorganisation för delade tjänster och köper Azure CSP delade tjänster-prenumerationen som ska användas för delade resurser och interna arbetsbelastningar.

   :::image type="content" source="images/sharedservices5.png" alt-text="Skapa klientorganisationen och köp prenumerationen.":::

## <a name="about-the-azure--internalshared-services-offer"></a>Om Azure – interna/delade tjänster erbjudande

- Prenumerationen Azure – interna/delade tjänster Azure är en ny typ av Azure-erbjudande i CSP som nås via Partnercenter och som partner får för sin egen användning av Azure.

- Azure Partner Shared Services prenumerationer är berättigade och kan användas för att köpa RU:er.

- Det Azure – interna/delade tjänster erbjudandet kan bara tillämpas på klientorganisationen för delade tjänster.

- Den främsta användningen för Azure – interna/delade tjänster-prenumerationen är så att du kan använda Azure i dina egna utvecklingssyften. Den delade klientorganisation som du använder för att etablera det här erbjudandet kan inte användas för andra tjänster, till exempel Office 365- eller Dynamics-licenser.

- Du kan avbryta prenumerationen precis som vilken annan prenumeration som helst. Gå till inställningarna **Visa alla**  >    >  **Delade tjänster**. Välj den Azure – interna/delade tjänster prenumerationen och avbryt den.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Åtkomst till Azure Partner Shared Services förbrukningsinformation

Du hittar Azure-förbrukningen på CSP-fakturan och avstämningsfilen. Den inkluderas som en del Microsoft Azure i radobjektet på fakturan. Den detaljerade förbrukningsinformationen blir tillgänglig i avstämningsfilen som loggas mot klienten som skapades för det här erbjudandet.

## <a name="azure-partner-shared-services-pricing"></a>Azure Partner Shared Services prissättning

Om du vill se den nya prisfilen för APSS går du till **Sälja** priser och erbjudanden  >   och väljer den aktuella månadens prislista. Under de kommande veckorna släpps även ett specifikt priskort-API.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Marketplace-erbjudanden och Azure Partner Shared Services

Från och med 1 mars 2019 stöder APSS inte längre Marketplace-erbjudanden.

|**Marketplace-support**   |**APSS stöds före 1 mars 2019**|**Efter den 1 mars 2019**|
|---------------------------|:----------------------------|:-------------------|
|Bring your own license (BYOL) och kostnadsfria tjänster   | Ja   | Inga|
|Andra Marketplace-erbjudanden från tredje part   | Inga   |Inga|

Partner som har BYOL eller kostnadsfria tjänster som distribueras med APSS påverkas inte. Efter den 1 mars 2019 kommer de dock inte att kunna köpa nya BYOL eller kostnadsfria tjänster.

Om du vill dra nytta av den fullständiga katalogen med Marketplace-erbjudanden (inte bara BYOL och kostnadsfria tjänster) rekommenderar vi att CSP-partner distribuerar delade tjänster med Azure-prenumerationer för web direct.  CSP-partner som tidigare har distribuerat BYOL från tredje part och kostnadsfria tjänstresurser från Marketplace och som vill fortsätta att använda dem och distribuera fler tredjepartserbjudanden uppmuntras att migrera APSS-prenumerationen till webb direktMigrering av [befintliga Azure-prenumerationer.](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)

Partner som planerar att fortsätta använda APSS-prenumerationen efter den 1 mars 2019 och vill distribuera nya [BYOL-tjänster](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) från tredje part eller kostnadsfria tjänster kan följa instruktionerna från ISV:er för att distribuera dem till sina APSS-prenumerationer.

## <a name="next-steps"></a>Nästa steg

- [Sälja programvaruprenumerationer via CSP](csp-software-subscriptions.md)