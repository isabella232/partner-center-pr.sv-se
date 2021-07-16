---
title: Exempelprogram
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd exempelprogrammet för att skapa ett eget program för att programmatiskt komma åt partnerinsiktsdata.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376943"
---
# <a name="sample-application"></a>Exempelprogram

Exempelprogram skapas i C# och JAVA-språk och är tillgängliga [på GitHub](https://github.com/partneranalytics)

- [C#-exempelprogram](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [JAVA-exempelprogram](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

Du kan välja att hämta inspiration från exempelprogrammet och skapa ditt eget program på val annat språk.

Exempelprogrammet uppnår följande mål:

- Genererar en Azure Active Directory-token (Azure AD).
- Hämtar tillgängliga datauppsättningar.
- Skapar användardefinierade frågor.
- Hämtar användardefinierade frågor och systemfrågor.
- Schemalägger en rapport.

Exempelprogrammet täcker inte metoden för att anropa API:er för andra funktioner. Processen för att anropa andra API:er förblir dock densamma som den som beskrivs ovan.

## <a name="how-to-run-the-application"></a>Så här kör du programmet

- Klona lagringsplatsen till ett lokalt system med följande kommando:

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> Mer information finns i filen ProgrammaticExportSampleAppMPN/README.md på GitHub [lagringsplatsen](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).

- Om du snabbt vill köra appen uppdaterar du klient-ID:t och klienthemligheten **iappsettings.Development.jspå**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Illustrera appsetting development json":::

När du kör appen startas en lokal webbserver och en sida öppnas ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Illustrerande användargränssnitt för exempelprogram":::

Den här sidan gör API-anrop till webbservern som körs på den lokala datorn, vilket i sin tur gör de faktiska API-anropen för programmeringsåtkomst.

## <a name="code-snippets"></a>Kodfragment

Den grundläggande strukturen i C#-koden för att göra API-anrop för programmatisk åtkomst är följande:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Illustrera kodfragment":::

## <a name="next-steps"></a>Nästa steg

[API:er för åtkomst till analysdata från partnerinsikter](insights-programmatic-analytics-available-api.md)
