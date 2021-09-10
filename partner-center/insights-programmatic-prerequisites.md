---
title: Krav för att komma åt analysdata programmatiskt
description: Krav för att komma åt analysdata programmatiskt
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 12c466cce37ac252fedf5f72ef90e390bb1af256
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960823"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Krav för att komma åt analysdata programmatiskt

**Lämpliga roller:** Globala | MPN-administratör

Innan du kan komma åt analysdata från partnerinsikter programmässigt måste du uppfylla följande krav.

## <a name="mpn-program-enrollment"></a>Registrering av MPN-program

För att komma åt partnerinsiktsanalysdata programmatiskt måste du vara registrerad i MPN-programmet och ha ett Partnercenter-konto. Mer information finns i Skapa [ett MPN-konto i Partnercenter](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Skapa Azure Active Directory (AAD)-program

Vanliga användarautentiseringsuppgifter kan inte användas för programmatisk åtkomst till Partner Insights Analytics-data. Ett Azure Active Directory (AAD)-program måste skapas tillsammans med en hemlighet (program - och användaråtkomst) för att få åtkomst till API:erna för programmatisk åtkomst. Information om hur du skapar ett AAD-program och en hemlighet finns [i Snabbstart: Registrera ett program med Microsofts identitetsplattform.](/azure/active-directory/develop/quickstart-register-app)   Behörighet krävs för åtkomst till Microsoft Partner-API. Information om hur du lägger till behörighet finns [i Partner-API autentisering – Partner](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Tilldela rollen Executive Report Viewer (ERV) till användaren

För att komma åt partnerinsiktsanalysdata programmatiskt bör du ha Executive Report Viewer (ERV). Information om hur du tilldelar EN ERV-roll till användaren finns [i Partnercenter Insights rollbaserad åtkomst – Partnercenter](insights-roles.md)

## <a name="generate-an-aad-token"></a>Generera en AAD-token

Du måste generera en AAD-token med program-ID:t (klienten), klienthemligheten, ditt användar-ID och lösenord.   [Gå hit för](insights-programmatic-first-api-call.md#token-generation) att få anvisningar om hur du skapar en AAD-token.

> [!Note]
> Token är giltig i en timme.

## <a name="next-steps"></a>Nästa steg
[Paradigm för programmatisk åtkomst](insights-programmatic-access-paradigm.md)