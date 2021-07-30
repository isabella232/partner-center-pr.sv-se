---
title: Insights Instrumentpanel för träning
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Utforska instrumentpanelen Utbildning i Partnercenter. Utbildning är en av de rapporter som är tillgängliga i området Partnercenter Insights (PCI).
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8749bdc1c2249f97d5db288f953eded1c4c06b02
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114843178"
---
# <a name="trainings-dashboard"></a>Instrumentpanel för träningar

**Lämpliga roller:** Användare av | Rapportvisningsprogram

Instrumentpanelen Utbildning ger insikter om certifieringar, utvärderingar och undersökningar som gjorts av företagets anställda. Instrumentpanelen Träningar innehåller följande avsnitt:

- Sammanfattning
- Träningsprestanda uppdelat efter certifieringar, utvärderingar och prov
- Individer efter autentiseringsuppgifter som certifieringar, utvärderingar och prov
- Aktivitetsinformation

>[!NOTE] 
>Den här rapporten är tillgänglig under Insights-hubben i Partnercenter. Om du vill visa den här rapporten bör du vara tilldelad rollen Rapportvisare eller Rapportvisningsprogram. Några få avsnitt i den här rapporten är bara synliga för användare som är användare av chefsrapport. Mer information om åtkomstkontroll för Insights finns i [PCI-roller.](insights-roles.md)

## <a name="summary"></a>Sammanfattning

I sammanfattningsavsnittet visas en numerisk ögonblicksbildsvy över olika prestandaindikatorer som är relaterade till dina träningar. De olika prestandaindikatorerna är certifierade individer, certifieringar, individer med provautentiseringsuppgifter, provautentiseringsuppgifter, individer med autentiseringsuppgifter för utvärdering och autentiseringsuppgifter för utvärdering. Data i det här avsnittet uppdateras baserat på det valda datumintervallet, som kan vara tre månader (3M), sex månader (6M) och 12 månader (1Y) eller ett anpassat dataintervall (anpassat). 

:::image type="content" source="images/insights/training-dashboard-summary.png" alt-text="Sammanfattning.":::

- **Individer med certifieringar:** representerar antalet distinkta personer med certifieringar i ditt företag.
- **Antal certifieringar:** representerar det totala antalet certifieringar som enskilda personer i företaget har tagit.
- **Personer med utvärderingar:** representerar antalet distinkta personer med autentiseringsuppgifter för utvärdering i ditt företag. 
- **Antal utvärderingar:** representerar det totala antalet utvärderingar som gjorts av enskilda personer i företaget.
- **Individer med undersökning:** representerar antalet distinkta individer med undersökningsautentiseringsuppgifter i företaget. 
- **Antal undersökningar:** representerar det totala antalet undersökningar som har tagits av individer i företaget.

## <a name="training-performance"></a>Träningsprestanda

Träningsprestanda visar antalet individer från månad till månad och de utbildningar som har slutförts av individer i företaget. Den delas upp efter certifieringar, utvärderingar och prov i form av ett diagram för det valda datumintervallet. X-axeln representerar månaderna för det valda datumintervallet. Y-axeln representerar det distinkta antalet individer och antalet träningsträningar som har tagits för den valda träningstypen. Välj respektive flikar ovanför diagrammet för att visa uppdelningen efter träningstyp. Diagramdata kan laddas ned via nedladdningsikonen i .tsv-format för det valda datumintervallet.

:::image type="content" source="images/insights/training-dashboard-training-performance.png" alt-text="Träningsprestanda.":::

## <a name="individuals-performance"></a>Individers prestanda

Avsnittet Individers prestanda visar information om den utbildning som enskilda personer i företaget har tagit för det valda datumintervallet. Sök och välj en individs namn i den vänstra panelen i avsnittet. Träningsinformationen för den valda personen visas på den högra panelen i avsnittet.

:::image type="content" source="images/insights/training-dashboard-individual-performance.png" alt-text="Enskilda prestanda.":::

>[!NOTE] 
> Avsnittet Prestanda för enskilda användare är endast tillgängligt för användare som visar chefsrapporten. 

## <a name="next-steps"></a>Nästa steg

[Rapporter i Partnercenter-Insights](partner-center-insights.md)

>[!NOTE] 
> Du kan ladda ned rådata som driver den här rapporten från avsnittet Ladda ned rapporter i Insights instrumentpanel. [Läs mer](insights-download-reports.md)