---
title: Exempelprogram
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Använd exempelprogrammet för att skapa ett eget program för att programmatiskt komma åt partnerinsiktsdata.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: c558852b7c2af7243187a856067d17a2137cfac867149b80e9c852a1d08d780a
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115683800"
---
# <a name="sample-application"></a>Exempelprogram

Exempelprogram skapas i C# och JAVA-språk och är tillgängliga på [GitHub](https://github.com/partneranalytics)

- [C#-exempelprogram](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [JAVA-exempelprogram](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

Du kan välja att hämta inspiration från exempelprogrammet och skapa ett eget program på val annat språk.

Exempelprogrammet uppnår följande mål:

- Genererar en Azure Active Directory -token (Azure AD).
- Hämtar tillgängliga datauppsättningar.
- Skapar användardefinierade frågor.
- Hämtar användardefinierade frågor och systemfrågor.
- Schemalägger en rapport.

Exempelprogrammet täcker inte metoden för att anropa API:er för andra funktioner. Processen för att anropa andra API:er förblir dock densamma som beskrivs ovan.

## <a name="how-to-run-the-application"></a>Så här kör du programmet

- Klona lagringsplatsen till ett lokalt system med det här kommandot:

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> Mer information finns i filen ProgrammaticExportSampleAppMPN/README.md på lagringsplatsen GitHub [.](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

- Om du snabbt vill köra appen uppdaterar du klient-ID:t och klienthemligheten **iappsettings.Development.jspå**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Illustrera json för appsetting-utveckling":::

Om du kör appen startas en lokal webbserver och en sida öppnas ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Illustrera användargränssnittet för exempelprogrammet":::

Den här sidan gör API-anrop till webbservern som körs på den lokala datorn, vilket i sin tur gör de faktiska API-anropen för programmeringsåtkomst.

## <a name="code-snippets"></a>Kodfragment

Den grundläggande strukturen i C#-koden för att göra API-anrop för programmatisk åtkomst är följande:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Illustrera kodfragment":::

## <a name="next-steps"></a>Nästa steg

[API:er för åtkomst till analysdata för partnerinsikter](insights-programmatic-analytics-available-api.md)
