---
title: Flytta kunder från aktuella Azure-erbjudanden till En Azure-plan
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig hur CSP-partner kan använda Partnercenter för att flytta kunder från befintliga CSP Azure-erbjudanden till Azure-tjänster enligt Azure-planen.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: eb9d88935bdc339c01ac47153c3d4a23047dc406
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960013"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Övergå kunder till Azure-plan från befintliga CSP Azure-erbjudanden

**Gäller för:** Partnercenter 

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Globala | Supportagent | Försäljningsagent | Administratör för användarhantering

Den här artikeln beskriver hur CSP-partner kan använda PartnerCenter för att flytta kunder från befintliga CSP Azure-erbjudanden till Azure-tjänster enligt Azure-planen. Indirekta leverantörer och direktfaktureringspartner kan övergå till den nya handelsupplevelsen som är tillgänglig i Microsoft Cloud Service Provider Program (CSP) för Azure. (Indirekta återförsäljare måste arbeta via sina indirekta leverantörer.) Kunderna får ett effektivt sätt att köpa molntjänster, oavsett om de köper från partner, från Microsoft-säljare eller direkt på webben.

Övergångsfunktionerna är endast för kunder som övergår till den nya handelsupplevelsen för Azure och som har signerat Microsoft-kundavtal. Det är inte för andra erbjudanden i CSP, till exempel Office 365 eller Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Övergå från befintliga CSP-erbjudanden till en Azure-plan

Du kan övergå från sina befintliga Azure-erbjudanden för molnlösningspartner till Azure-tjänster enligt Azure-planen i den nya handelsupplevelsen i CSP-programmet från Partnercenter. För att göra detta måste partnern och kunden ha en etablerad återförsäljarrelation via Partnercenter och kunden måste ha signerat Microsoft-kundavtal.

### <a name="select-transition-to-azure-plan"></a>Välj övergång till Azure-plan

1. Välj Azure-plan för din kund.

2. Välj **Transition billing to Azure plan (Övergå fakturering till Azure-plan).**

   :::image type="content" source="images/azure/transition1.png" alt-text="Skärmbild som visar rapportinformation om användningsbaserade prenumerationer med ett valbart alternativ som heter: Övergå från Azure-prenumerationsfakturering till Azure-plan.":::

3. Välj **Fortsätt**

   :::image type="content" source="images/azure/transition2.png" alt-text="Dialogruta med rubriken Övergång till Azure-plan med effekter att läsa om övergången och två alternativ att välja, Fortsätt eller Avbryt.":::

   Kunden övergår till Azure-planen.

   **Övergångsarbetsflödet automatiserar de nödvändiga stegen:**

   - Köp av Azure-planer
   - En plan per kund i scenarier med direkt CSP  
   - En plan per återförsäljare  

   En partner har till exempel köpt två Microsoft Azure erbjudanden och har tagit med två distinktaPOR i köpet. I det här fallet köper övergångsarbetsflödet två Azure-planer (en per återförsäljare) och mappar de respektive Azure-prenumerationerna under Azure-planerna automatiskt.  

   **Mappa Azure-prenumeration till Azure-plan**

   När du har köpt Azure-prenumerationerna mappar vårt system de befintliga Azure-prenumerationerna till Azure-planerna. Förloppet kan visas i Azure Portal samt i Partnercenter.

4. Gå tillbaka till kundens **partnercenterprenumerationer för** att uppdatera budgetgränsen med hjälp av den lokala valutan.

   :::image type="content" source="images/azure/transition3.png" alt-text="Partiell vy av sidan Partnercenter-prenumerationer med budgetgränser som angetts i lokal valuta för en faktureringsperiod.":::

   >[!NOTE]
   >Budgeten som du anger i Partnercenter förs inte över till Azure Portal. Du bör också ange budget och avisering i Azure Portal.

   När du flyttar till Azure-planen kan du inte längre köpa Azure-prenumerationer för den här kunden. Du skapar prenumerationerna under Azure-planen i Azure Portal.

   >[!NOTE]
   > Alla Azure-prenumerationer som köpts via RBAC enligt Azure-planen prissätts och faktureras i lokal valuta. FX-priser används inte.

### <a name="track-your-transition-details"></a>Spåra din övergångsinformation

Följ övergångsförloppet i Azure Portal samt i Partnercenter.

:::image type="content" source="images/azure/details1.png" alt-text="Skärmbild som visar en tabell med en lista över övergångsinformation per prenumeration – inklusive prenumerations-ID, övergångsdatum och övergångsstatus.":::

### <a name="billing-impact-to-partners"></a>Faktureringspåverkan till partner

Om du övergår till en kund från ett befintligt Azure-erbjudande för molnlagring får du följande faktureringspåverkan:

- Du debiteras på din befintliga CSP-faktura för all användning fram till den tidpunkt då du avslutar den ursprungliga CSP Azure-prenumerationen.

- Om du hade administratörsbehörighet till den befintliga CSP-prenumerationen kommer du att fortsätta att ha åtkomst när prenumerationen migreras.

Om du vill övergå direkt till Enterprise-avtal till CSP- och server- och molnregistreringar till Azure-tjänster läser du Få faktureringsägarskap för [Azure-prenumerationer för Microsoft-partneravtal](/azure/billing/mpa-request-ownership)

### <a name="audit-log"></a>Granskningslogg

Om du vill stämma av faktureringen visar du din historik över Microsoft Azure prenumerationer (0145P) på **sidan** Prenumerationer.

Prenumerationen "Microsoft Azure" (0145P) består av två delar:

1. Handelsprenumeration
2. Azure-prenumeration (berättigande)

När övergången är klar flyttas Azure-prenumerationen under den nya Azure-planen och handelsprenumerationen inaktiveras så att ingen ytterligare användning rapporteras.  

>[!NOTE]
>När Microsoft Azure-prenumeration (0145P) köps i CSP har både handelsprenumerationen och Azure-prenumerationen (berättigandet) samma värde. Det är bara om faktureringsägarskapet ändras eller överföringar skiljer sig värdena åt.

### <a name="transition-issues"></a>Problem med övergången

Vi förväntar oss inte några problem under övergångar. Om det inträffar uppdaterar vi dig i själva övergångsarbetsflödet. Det kommer inte att finnas några problem med Azure-användning.  

## <a name="next-steps"></a>Nästa steg

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)

- [Partner-intjänad kredit – översikt](partner-earned-credit.md)
