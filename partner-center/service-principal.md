---
title: Azure AD-tjänstens huvudnamn
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ta reda på hur du lägger till ett huvudnamn för tjänsten i din Azure AD-klientorganisation. Det innebär att du lägger till ett Azure AD-program (tjänstens huvudnamn) i Partnercenter.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 3698032a632384e8416664c9564819d7c4da9c38
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551562"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="92477-104">Lägga till ett Azure AD-program (tjänstens huvudnamn) i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="92477-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="92477-105">**Lämpliga roller:** Global administratör</span><span class="sxs-lookup"><span data-stu-id="92477-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="92477-106">I programmet för den kommersiella marknadsplatsen i Partnercenter kan du nu lägga till ett Microsoft Azure Active Directory-program (Azure AD) (tjänstens huvudnamn) som en användare i ditt Partnercenter-konto.</span><span class="sxs-lookup"><span data-stu-id="92477-106">In the Commercial Marketplace program in Partner Center, you are now able to add a Microsoft Azure Active Directory (Azure AD) application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="92477-107">(Du kunde göra det tidigare i ditt Cloud Partner Portal-konto (CPP).</span><span class="sxs-lookup"><span data-stu-id="92477-107">(You were able to do so previously in your Cloud Partner Portal (CPP) account.</span></span> <span data-ttu-id="92477-108">Nu när du har migrerat till Partnercenter är CPP-kontot skrivskyddat.)</span><span class="sxs-lookup"><span data-stu-id="92477-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="92477-109">Tjänstens huvudnamn är synonymt med Azure AD-programmet.</span><span class="sxs-lookup"><span data-stu-id="92477-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="92477-110">Lägga till ett Azure AD-program (tjänstens huvudnamn)</span><span class="sxs-lookup"><span data-stu-id="92477-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="92477-111">Från instrumentpanelen i Partnercenter väljer **du Inställningar** och sedan Inställningar **för utvecklare.**</span><span class="sxs-lookup"><span data-stu-id="92477-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="92477-112">Välj **Användare** och sedan Lägg **till Azure AD-program.**</span><span class="sxs-lookup"><span data-stu-id="92477-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="92477-113">Välj ett befintligt Azure AD-program eller skapa ett nytt.</span><span class="sxs-lookup"><span data-stu-id="92477-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="92477-114">Om du skapar ett nytt Azure AD-program ska du inkludera följande information:</span><span class="sxs-lookup"><span data-stu-id="92477-114">If you create a new Azure AD application, include the following information:</span></span>  

   - <span data-ttu-id="92477-115">**Svars-URL:** Den URL där användare kan logga in för att använda ditt Azure AD-program.</span><span class="sxs-lookup"><span data-stu-id="92477-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="92477-116">**App-ID-URI:** En logisk identifierare för Azure AD-programmet som visas när den skickar en begäran om enkel inloggning till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="92477-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="92477-117">**Säkerhetsroller:** Rollhanteraren **(samma** som rollen Ägare i CPP) och Utvecklare **(samma** som rollen Deltagare i CPP) gäller för programmet För kommersiell marknadsplats i Partnercenter och kan associeras med det här Azure AD-programmet.</span><span class="sxs-lookup"><span data-stu-id="92477-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="92477-118">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="92477-118">Next steps</span></span>

- [<span data-ttu-id="92477-119">Översikt över den kommersiella marknadsplatsen i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="92477-119">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)