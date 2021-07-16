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
# <a name="sample-application"></a><span data-ttu-id="84632-103">Exempelprogram</span><span class="sxs-lookup"><span data-stu-id="84632-103">Sample Application</span></span>

<span data-ttu-id="84632-104">Exempelprogram skapas i C# och JAVA-språk och är tillgängliga [på GitHub](https://github.com/partneranalytics)</span><span class="sxs-lookup"><span data-stu-id="84632-104">Sample applications are created in C# and JAVA languages and are available on [GitHub](https://github.com/partneranalytics)</span></span>

- [<span data-ttu-id="84632-105">C#-exempelprogram</span><span class="sxs-lookup"><span data-stu-id="84632-105">C# Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [<span data-ttu-id="84632-106">JAVA-exempelprogram</span><span class="sxs-lookup"><span data-stu-id="84632-106">JAVA Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

<span data-ttu-id="84632-107">Du kan välja att hämta inspiration från exempelprogrammet och skapa ditt eget program på val annat språk.</span><span class="sxs-lookup"><span data-stu-id="84632-107">You can choose to take inspiration from the sample application and build your own application in any language.</span></span>

<span data-ttu-id="84632-108">Exempelprogrammet uppnår följande mål:</span><span class="sxs-lookup"><span data-stu-id="84632-108">The sample application achieves the following objectives:</span></span>

- <span data-ttu-id="84632-109">Genererar en Azure Active Directory-token (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="84632-109">Generates an Azure Active Directory (Azure AD) Token.</span></span>
- <span data-ttu-id="84632-110">Hämtar tillgängliga datauppsättningar.</span><span class="sxs-lookup"><span data-stu-id="84632-110">Gets available datasets.</span></span>
- <span data-ttu-id="84632-111">Skapar användardefinierade frågor.</span><span class="sxs-lookup"><span data-stu-id="84632-111">Creates user defined queries.</span></span>
- <span data-ttu-id="84632-112">Hämtar användardefinierade frågor och systemfrågor.</span><span class="sxs-lookup"><span data-stu-id="84632-112">Gets user defined and system queries.</span></span>
- <span data-ttu-id="84632-113">Schemalägger en rapport.</span><span class="sxs-lookup"><span data-stu-id="84632-113">Schedules a report.</span></span>

<span data-ttu-id="84632-114">Exempelprogrammet täcker inte metoden för att anropa API:er för andra funktioner.</span><span class="sxs-lookup"><span data-stu-id="84632-114">The sample application doesn't cover the method of calling APIs for other functionalities.</span></span> <span data-ttu-id="84632-115">Processen för att anropa andra API:er förblir dock densamma som den som beskrivs ovan.</span><span class="sxs-lookup"><span data-stu-id="84632-115">However, the process of calling other APIs remains the same as outlined above.</span></span>

## <a name="how-to-run-the-application"></a><span data-ttu-id="84632-116">Så här kör du programmet</span><span class="sxs-lookup"><span data-stu-id="84632-116">How to run the application</span></span>

- <span data-ttu-id="84632-117">Klona lagringsplatsen till ett lokalt system med följande kommando:</span><span class="sxs-lookup"><span data-stu-id="84632-117">Clone the repository to a local system using this command:</span></span>

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> <span data-ttu-id="84632-118">Mer information finns i filen ProgrammaticExportSampleAppMPN/README.md på GitHub [lagringsplatsen](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span><span class="sxs-lookup"><span data-stu-id="84632-118">For more instructions, refer to the ProgrammaticExportSampleAppMPN/README.md file in the GitHub [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span></span>

- <span data-ttu-id="84632-119">Om du snabbt vill köra appen uppdaterar du klient-ID:t och klienthemligheten **iappsettings.Development.jspå**</span><span class="sxs-lookup"><span data-stu-id="84632-119">To quickly run the app, update the client id and client secret in the **appsettings.Development.json**</span></span>

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Illustrera appsetting development json":::

<span data-ttu-id="84632-121">När du kör appen startas en lokal webbserver och en sida öppnas ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).</span><span class="sxs-lookup"><span data-stu-id="84632-121">Running the app will start a local web server and a page will open (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span></span>
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Illustrerande användargränssnitt för exempelprogram":::

<span data-ttu-id="84632-123">Den här sidan gör API-anrop till webbservern som körs på den lokala datorn, vilket i sin tur gör de faktiska API-anropen för programmeringsåtkomst.</span><span class="sxs-lookup"><span data-stu-id="84632-123">This page will make API calls to the webserver running on the local machine, which in turn will make the actual programmatic access API calls.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="84632-124">Kodfragment</span><span class="sxs-lookup"><span data-stu-id="84632-124">Code Snippets</span></span>

<span data-ttu-id="84632-125">Den grundläggande strukturen i C#-koden för att göra API-anrop för programmatisk åtkomst är följande:</span><span class="sxs-lookup"><span data-stu-id="84632-125">The basic structure of the C# code for doing the programmatic access API calls is as follows:</span></span>
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Illustrera kodfragment":::

## <a name="next-steps"></a><span data-ttu-id="84632-127">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="84632-127">Next steps</span></span>

[<span data-ttu-id="84632-128">API:er för åtkomst till analysdata från partnerinsikter</span><span class="sxs-lookup"><span data-stu-id="84632-128">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
