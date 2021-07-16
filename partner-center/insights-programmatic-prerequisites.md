---
title: Krav för att programmatiskt få åtkomst till analysdata
description: Krav för att programmatiskt få åtkomst till analysdata
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376952"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Krav för att programmatiskt få åtkomst till analysdata

**Lämpliga roller:** Global | MPN-administratör

Innan du kan komma åt analysdata för partnerinsikter programmatiskt måste du uppfylla följande krav.

## <a name="mpn-program-enrollment"></a>MPN-programregistrering

För att komma åt analysdata för partnerinsikter programmatiskt måste du vara registrerad i MPN-programmet och ha ett Partnercenter-konto. Mer information finns i Skapa [ett MPN-konto i Partnercenter](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Skapa Azure Active Directory (AAD)-program

Vanliga användarautentiseringsuppgifter kan inte användas för programmatisk åtkomst till Partner Insights Analytics-data. Ett Azure Active Directory (AAD)-program måste skapas tillsammans med en hemlighet (program - och användaråtkomst) för att få åtkomst till API:erna för programmatisk åtkomst. Information om hur du skapar ett AAD-program och en hemlighet finns [i Snabbstart: Registrera ett program med Microsofts identitetsplattform.](/azure/active-directory/develop/quickstart-register-app)   Behörighet krävs för åtkomst till Microsoft Partner-API. Information om hur du lägger till behörighet finns i [Partner-API autentisering – Partner](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Tilldela rollen som chefsrapportvisare (ERV) till användaren

Om du vill komma åt analysdata för partnerinsikter programmatiskt bör du ha ERV (Executive Report Viewer). Information om hur du tilldelar ANVÄNDAREN EN ERV-roll finns [i Partnercenter Insights rollbaserad åtkomst – Partnercenter](insights-roles.md)

## <a name="generate-an-aad-token"></a>Generera en AAD-token

Du måste generera en AAD-token med program-ID:t (klienten), klienthemligheten, ditt användar-ID och lösenord.   [Här finns anvisningar](insights-programmatic-first-api-call.md#token-generation) om hur du genererar en AAD-token.

> [!Note]
> Token är giltig i en timme.

## <a name="next-steps"></a>Nästa steg
[Paradigm för programmatisk åtkomst](insights-programmatic-access-paradigm.md)