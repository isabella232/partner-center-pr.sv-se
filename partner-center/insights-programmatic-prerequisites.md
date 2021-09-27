---
title: Krav för att programmatiskt få åtkomst till analysdata
description: Krav för att programmatiskt få åtkomst till analysdata
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 9359cb25fee113ee166c7ce407ed70f319f3e6b6
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129071094"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Krav för att programmatiskt få åtkomst till analysdata

**Lämpliga roller:** Global | MPN-administratör

Innan du kan komma åt analysdata från partnerinsikter programmatiskt måste du uppfylla följande krav.

## <a name="mpn-program-enrollment"></a>Registrering av MPN-program

För att komma åt partnerinsiktsanalysdata programmatiskt måste du vara registrerad i MPN-programmet och ha ett Partnercenter-konto. Mer information finns i Skapa [ett MPN-konto i Partnercenter](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Skapa Azure Active Directory (AAD)-program

Vanliga användarautentiseringsuppgifter kan inte användas för programmatisk åtkomst till Partner Insights Analytics-data. Ett Azure Active Directory (AAD)-program måste skapas tillsammans med en hemlighet (program - och användaråtkomst) för att få åtkomst till API:erna för programmatisk åtkomst. Information om hur du skapar ett AAD-program och en hemlighet finns i [Snabbstart: Registrera ett program med Microsofts identitetsplattform.](/azure/active-directory/develop/quickstart-register-app)   Behörighet krävs för åtkomst till Microsoft Partner-API. Information om hur du lägger till behörighet finns [i Partner-API autentisering – Partner](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Tilldela rollen Executive Report Viewer (ERV) till användaren

För att komma åt partnerinsiktsanalysdata programmatiskt bör du ha Executive Report Viewer (ERV). Information om hur du tilldelar en ERV-roll till användaren finns [i Partnercenter Insights rollbaserad åtkomst – Partnercenter](insights-roles.md)

## <a name="generate-an-aad-token"></a>Generera en AAD-token

Du måste generera en AAD-token med program-ID:t (klienten), klienthemligheten, ditt användar-ID och lösenord.   [Gå hit för](insights-programmatic-first-api-call.md#token-generation) att få anvisningar om hur du genererar en AAD-token.

> [!Note]
> Token är giltig i en timme.

## <a name="next-steps"></a>Nästa steg
[Paradigm för programmatisk åtkomst](insights-programmatic-access-paradigm.md)