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
# <a name="prerequisites-to-programmatically-access-analytics-data"></a><span data-ttu-id="ae466-103">Krav för att programmatiskt få åtkomst till analysdata</span><span class="sxs-lookup"><span data-stu-id="ae466-103">Prerequisites to programmatically access analytics data</span></span>

<span data-ttu-id="ae466-104">**Lämpliga roller:** Global | MPN-administratör</span><span class="sxs-lookup"><span data-stu-id="ae466-104">**Appropriate roles:** Global admin | MPN admin</span></span>

<span data-ttu-id="ae466-105">Innan du kan komma åt analysdata för partnerinsikter programmatiskt måste du uppfylla följande krav.</span><span class="sxs-lookup"><span data-stu-id="ae466-105">Before you can programmatically access partner insights analytics data, you need to meet the following requirements.</span></span>

## <a name="mpn-program-enrollment"></a><span data-ttu-id="ae466-106">MPN-programregistrering</span><span class="sxs-lookup"><span data-stu-id="ae466-106">MPN Program enrollment</span></span>

<span data-ttu-id="ae466-107">För att komma åt analysdata för partnerinsikter programmatiskt måste du vara registrerad i MPN-programmet och ha ett Partnercenter-konto.</span><span class="sxs-lookup"><span data-stu-id="ae466-107">To access partner insights analytics data programmatically, you need to be enrolled in the MPN program and have a Partner Center account.</span></span> <span data-ttu-id="ae466-108">Mer information finns i Skapa [ett MPN-konto i Partnercenter](mpn-create-a-partner-center-account.md)</span><span class="sxs-lookup"><span data-stu-id="ae466-108">To learn how, see [Create an MPN account in Partner Center](mpn-create-a-partner-center-account.md)</span></span>

## <a name="create-azure-active-directory-aad-application"></a><span data-ttu-id="ae466-109">Skapa Azure Active Directory (AAD)-program</span><span class="sxs-lookup"><span data-stu-id="ae466-109">Create Azure Active Directory (AAD) application</span></span>

<span data-ttu-id="ae466-110">Vanliga användarautentiseringsuppgifter kan inte användas för programmatisk åtkomst till Partner Insights Analytics-data.</span><span class="sxs-lookup"><span data-stu-id="ae466-110">Regular user credentials cannot be used for programmatic access of Partner Insights Analytics data.</span></span> <span data-ttu-id="ae466-111">Ett Azure Active Directory (AAD)-program måste skapas tillsammans med en hemlighet (program - och användaråtkomst) för att få åtkomst till API:erna för programmatisk åtkomst.</span><span class="sxs-lookup"><span data-stu-id="ae466-111">An Azure Active Directory (AAD) application needs to be created along with a secret (application + user access) to access the programmatic access APIs.</span></span> <span data-ttu-id="ae466-112">Information om hur du skapar ett AAD-program och en hemlighet finns [i Snabbstart: Registrera ett program med Microsofts identitetsplattform.](/azure/active-directory/develop/quickstart-register-app)   Behörighet krävs för åtkomst till Microsoft Partner-API.</span><span class="sxs-lookup"><span data-stu-id="ae466-112">To learn how to create an AAD application and secret, see [Quickstart: Register an application with the Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app) Permission is required to access Microsoft Partner API.</span></span> <span data-ttu-id="ae466-113">Information om hur du lägger till behörighet finns i [Partner-API autentisering – Partner](/partner/develop/api-authentication#application-and-user-access)</span><span class="sxs-lookup"><span data-stu-id="ae466-113">To learn how to add permission, see [Partner API authentication - Partner](/partner/develop/api-authentication#application-and-user-access)</span></span>

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a><span data-ttu-id="ae466-114">Tilldela rollen som chefsrapportvisare (ERV) till användaren</span><span class="sxs-lookup"><span data-stu-id="ae466-114">Assign Executive Report Viewer (ERV) role to the user</span></span>

<span data-ttu-id="ae466-115">Om du vill komma åt analysdata för partnerinsikter programmatiskt bör du ha ERV (Executive Report Viewer).</span><span class="sxs-lookup"><span data-stu-id="ae466-115">To access partner insights analytics data programmatically, you should have Executive Report Viewer (ERV).</span></span> <span data-ttu-id="ae466-116">Information om hur du tilldelar ANVÄNDAREN EN ERV-roll finns [i Partnercenter Insights rollbaserad åtkomst – Partnercenter](insights-roles.md)</span><span class="sxs-lookup"><span data-stu-id="ae466-116">To learn how to assign ERV role to the user, see [Partner Center Insights role-based access - Partner Center](insights-roles.md)</span></span>

## <a name="generate-an-aad-token"></a><span data-ttu-id="ae466-117">Generera en AAD-token</span><span class="sxs-lookup"><span data-stu-id="ae466-117">Generate an AAD token</span></span>

<span data-ttu-id="ae466-118">Du måste generera en AAD-token med program-ID:t (klienten), klienthemligheten, ditt användar-ID och lösenord.   [Här finns anvisningar](insights-programmatic-first-api-call.md#token-generation) om hur du genererar en AAD-token.</span><span class="sxs-lookup"><span data-stu-id="ae466-118">You need to Generate an AAD token using the Application (client) ID, client secret, your user ID and password.  [Check here](insights-programmatic-first-api-call.md#token-generation) for steps to generate AAD token.</span></span>

> [!Note]
> <span data-ttu-id="ae466-119">Token är giltig i en timme.</span><span class="sxs-lookup"><span data-stu-id="ae466-119">The token is valid for one hour.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ae466-120">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ae466-120">Next steps</span></span>
[<span data-ttu-id="ae466-121">Paradigm för programmatisk åtkomst</span><span class="sxs-lookup"><span data-stu-id="ae466-121">Programmatic access paradigm</span></span>](insights-programmatic-access-paradigm.md)