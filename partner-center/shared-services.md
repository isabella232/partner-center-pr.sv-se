---
title: Lägga till Azure Partner Shared Services
description: Använd Azure Partner Shared Services att köpa Azure-prenumerationer för eget bruk och för att ha en enhetlig metod för att köpa, spåra och hantera Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 35c5d378f66071f3c97abdf74eec27e78a8ac778
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114842056"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Lägg Azure Partner Shared Services så att partner kan köpa Azure-prenumerationer för eget bruk

**Lämpliga roller:** Global | Administratörsagent | Försäljningsagent

Azure Partner Shared Services (APSS) är en ny erbjudandetyp för partner i Molnlösningsleverantör-programmet (CSP), vilket gör det möjligt för partner att köpa Azure-prenumerationer för eget bruk.Det skapar en möjlighet för partner att använda en enhetlig metod för att köpa, spåra och hantera Azure, utöver möjligheten att konsolidera sina Azure-licensierings- och vidareförsäljningsavtal med Microsoft. Med APSS har partner nu samma flexibilitet att använda Azure-prenumerationer i CSP som de gör i Microsoft företagsavtal- och Web Direct-program, vilket öppnar scenarier som: skapa utvecklings- och testmiljöer, distribuera interna arbetsbelastningar och vara värd för delade tjänster eller program med flera innehavare.  

## <a name="create-the-shared-services-tenant"></a>Skapa klientorganisationen för delade tjänster

1. Gå till **Inställningar**  >  **kontoinställningar**  >  **Delade tjänster.**

   :::image type="content" source="images/sharedservices2.png" alt-text="Kontoinställningar > delade tjänster":::

2. Om du inte redan har en klientorganisation för delade tjänster väljer du **Skapa delade tjänster.**

   :::image type="content" source="images/sharedservices3.png" alt-text="Skapa delade tjänster.":::

3. Detta skapar en klientorganisation för delade tjänster och köper Azure CSP Shared Services-prenumerationen som ska användas för delade resurser och intern arbetsbelastning.

   :::image type="content" source="images/sharedservices5.png" alt-text="Skapa klientorganisationen och köp prenumerationen.":::

## <a name="about-the-azure--internalshared-services-offer"></a>Om Azure – interna/delade tjänster erbjudandet

- Prenumerationen Azure – interna/delade tjänster en ny Azure-erbjudandetyp i CSP som nås via Partnercenter och som partner får för sin egen användning av Azure.

- Azure Partner Shared Services prenumerationer är berättigade och kan användas för att köpa RU:er.

- Det Azure – interna/delade tjänster erbjudandet kan endast tillämpas på klientorganisationen för delade tjänster.

- Den primära användningen för Azure – interna/delade tjänster-prenumerationen är så att du kan använda Azure i dina egna utvecklingssyften. Den delade klientorganisation som du använder för att etablera det här erbjudandet kan inte användas för andra tjänster som Office 365 eller Dynamics-licenser.

- Du kan avbryta prenumerationen precis som vilken annan prenumeration som helst. Gå till inställningarna **Visa alla**  >    >  **Delade tjänster**. Välj Azure – interna/delade tjänster prenumeration och avbryt den.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Åtkomst till Azure Partner Shared Services förbrukningsinformation

Du hittar Azure-förbrukningen på CSP-fakturan och avstämningsfilen. Den inkluderas som en del Microsoft Azure på fakturan. Den detaljerade förbrukningsinformationen kommer att vara tillgänglig i avstämningsfilen som loggats mot den klientorganisation som skapades för erbjudandet.

## <a name="azure-partner-shared-services-pricing"></a>Azure Partner Shared Services prissättning

Om du vill se den nya prisfilen för APSS går du till **Säljpriser** och erbjudanden  >   och väljer den aktuella månadens prislista. Under de kommande veckorna släpps även ett specifikt priskort-API.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Marketplace-erbjudanden och Azure Partner Shared Services

Från och med 1 mars 2019 stöder APSS inte längre Marketplace-erbjudanden.

|**Marketplace-support**   |**APSS stöds före 1 mars 2019**|**Efter den 1 mars 2019**|
|---------------------------|:----------------------------|:-------------------|
|Bring your own license (BYOL) och kostnadsfria tjänster   | Ja   | Inga|
|Andra marketplace-erbjudanden från tredje part   | Inga   |Inga|

Partner som har BYOL eller kostnadsfria tjänster som distribueras med APSS påverkas inte. Efter den 1 mars 2019 kommer de dock inte att kunna köpa nya BYOL-tjänster eller kostnadsfria tjänster.

Om du vill dra nytta av den fullständiga katalogen med Marketplace-erbjudanden (inte bara BYOL och kostnadsfria tjänster) rekommenderar vi att CSP-partner distribuerar delade tjänster med Azure-prenumerationer för web direct.  CSP-partner som tidigare har distribuerat BYOL från tredje part och kostnadsfria tjänstresurser från Marketplace och vill fortsätta att använda dem och distribuera fler tredjepartserbjudanden uppmanas att migrera APSS-prenumerationen till webb direktMigrering av befintliga [Azure-prenumerationer.](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)

Partner som planerar att fortsätta använda APSS-prenumerationen efter den 1 mars 2019 och vill distribuera nya [BYOL-tjänster](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) från tredje part eller kostnadsfria tjänster kan följa instruktionerna från ISV:er för att distribuera dem till sina APSS-prenumerationer.

## <a name="next-steps"></a>Nästa steg

- [Sälja programvaruprenumerationer via CSP](csp-software-subscriptions.md)