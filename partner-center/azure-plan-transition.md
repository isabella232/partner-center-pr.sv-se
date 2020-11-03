---
title: Flytta kunder från nuvarande Azure-erbjudanden till Azure-prenumerationen
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur CSP-partner kan använda Partner Center för att flytta kunder från befintliga CSP Azure-erbjudanden till Azure-tjänster under Azure-prenumerationen.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 5390e950689e930b246aaaddcb1a9ef1b1ab6d46
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531633"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Överföring av kunder till Azure-plan från befintliga CSP Azure-erbjudanden

**Lämpliga roller**

- Administratörs agent
- Faktureringsadministratör
- Global administratör
- Support agent
- Försäljnings agent
- Administratör för användar hantering

Indirekta leverantörer och direkta fakturerings partner kan övergå till den nya Commerce-upplevelsen som finns i Microsoft Cloud Service Provider-program (CSP) för Azure. (Indirekta åter försäljare måste arbeta via sina indirekta leverantörer.) Kunder kommer att ha ett förenklat sätt att köpa moln tjänster, om de köper från partner, från Microsoft-säljare eller direkt på webben.

Över gångs funktionen är endast till för kunder som övergår till den nya Commerce-upplevelsen för Azure och som har undertecknat Microsofts kund avtal och inte för andra erbjudanden i CSP som Office 365 eller Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Över gång av befintliga CSP-erbjudanden till en Azure-plan

Du kan överföra en kund från sina befintliga CSP Azure-erbjudanden till Azure-tjänster under Azure-planen i den nya Commerce-upplevelsen i CSP-programmet inifrån Partner Center. För att göra detta måste partnern och kunden ha en etablerad åter försäljares relation via partner Center och kunden måste ha undertecknat Microsofts kund avtal.

### <a name="select-transition-to-azure-plan"></a>Välj över gång till Azure-plan

1. Välj Azure-plan för din kund.

2. Välj **över gångs fakturering till Azure-plan** .

   :::image type="content" source="images/azure/transition1.png" alt-text="Skärm bild som visar rapport information om användnings prenumerationer med ett valbart alternativ som kallas: överför Azure-prenumerations fakturering till Azure-plan.":::

3. Välj **Fortsätt**

   :::image type="content" source="images/azure/transition2.png" alt-text="Skärm bild som visar rapport information om användnings prenumerationer med ett valbart alternativ som kallas: överför Azure-prenumerations fakturering till Azure-plan.":::

   Kunden kommer att överföras till Azure-prenumerationen.

   **Över gångs arbets flödet automatiserar de nödvändiga stegen** :

   - Köp av Azure-plan (er)
   - En plan per kund i direkta CSP-scenarier  
   - En plan per åter försäljare  

   Till exempel har en partner köpt två Microsoft Azure erbjudanden och har inkluderat två distinkta POR i köpet. I det här fallet kommer över gångs arbets flödet att köpa två Azure-planer (ett per åter försäljare) och mappa respektive Azure-prenumerationer i Azure-prenumerationerna automatiskt.  

   **Mappa Azure-prenumeration till Azure-plan**

   Efter ditt köp av Azure-plan (er) mappar vårt system de befintliga Azure-prenumerationerna till Azure-prenumerationerna. Förloppet kan visas i Azure Portal såväl som i Partner Center.

4. Gå tillbaka till kundns Partner Center- **prenumerationer** för att uppdatera budget gränsen med hjälp av sin lokala valuta.

   :::image type="content" source="images/azure/transition3.png" alt-text="Skärm bild som visar rapport information om användnings prenumerationer med ett valbart alternativ som kallas: överför Azure-prenumerations fakturering till Azure-plan.":::

   >[!NOTE]
   >Den budget som du ställer in i Partner Center överför inte till Azure Portal. Du bör också ställa in budget och avisering i Azure Portal.

   När du flyttar till Azure-planen kan du inte längre köpa Azure-prenumerationer för den här kunden. Du skapar prenumerationerna under Azure-planen i Azure Portal.

   >[!NOTE]
   > Alla Azure-prenumerationer som köpts via RBAC under Azure-Abonnemanget debiteras och faktureras i lokal valuta. FX-priser kommer inte att användas.

### <a name="track-your-transition-details"></a>Spåra din över gångs information

Följ över gångs förloppet i Azure Portal såväl som i Partner Center.

:::image type="content" source="images/azure/details1.png" alt-text="Skärm bild som visar rapport information om användnings prenumerationer med ett valbart alternativ som kallas: överför Azure-prenumerations fakturering till Azure-plan.":::

### <a name="billing-impact-to-partners"></a>Fakturerings påverkan för partner

Om du övergår till en kund från ett befintligt Azure-erbjudande för CSP, kommer du att ha följande fakturerings påverkan:

- Du debiteras på din befintliga CSP-faktura för all användning fram till den tidpunkt då den ursprungliga CSP Azure-prenumerationen avslutas.

- Om du har administratörs behörighet för den befintliga CSP-prenumerationen fortsätter du att ha åtkomst när prenumerationen migreras.

Om du vill överföra direkta Enterprise-avtal till CSP och server-och moln registreringar till Azure-tjänster läser du [få fakturerings ägande av Azure-prenumerationer för Microsoft partner Agreement](/azure/billing/mpa-request-ownership)

### <a name="audit-log"></a>Granskningslogg

För att stämma av faktureringen, se historiken för "Microsoft Azure"-prenumerationer (0145P) på **prenumerations** sidan.

"Microsoft Azure-prenumerationen (0145P) består av två delar:

1. Handels prenumeration
2. Azure-prenumeration (berättigande)

När över gången är klar flyttas Azure-prenumerationen under den nya Azure-planen och handels prenumerationen inaktive ras så att ingen ytterligare användning rapporteras.  

>[!NOTE]
>När Microsoft Azure (0145P)-prenumerationen köps i CSP har både handels prenumerationen och Azure-prenumerationen samma värde. Det är bara vid fakturering av ägande rätt ändringar eller överföringar som gör värdena annorlunda.

### <a name="transition-issues"></a>Övergångs problem

Vi förväntar sig inga problem under över gången. Om ett sådant inträffar kommer vi att uppdatera dig i över gångs arbets flödet. Det uppstår inga störningar på användningen av Azure.  

## <a name="next-steps"></a>Nästa steg

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)

- [Partner intjänad kredit – översikt](partner-earned-credit.md)