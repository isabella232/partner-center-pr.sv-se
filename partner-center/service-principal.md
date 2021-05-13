---
title: Azure AD-tjänstens huvudnamn
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du lägger till ett huvudnamn för tjänsten i din Azure AD-klientorganisation. Det innebär att du lägger till ett Azure AD-program (tjänstens huvudnamn) i Partnercenter.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d12bb66574e6bcee60b2a1df1673dc9171fbee2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854935"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="f104b-104">Lägga till ett Azure AD-program (tjänstens huvudnamn) i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="f104b-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="f104b-105">**Lämpliga roller:** Global administratör</span><span class="sxs-lookup"><span data-stu-id="f104b-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="f104b-106">I Commercial Marketplace-programmet i Partnercenter kan du nu lägga till ett Azure AD-program (tjänstens huvudnamn) som en användare i ditt Partnercenter-konto.</span><span class="sxs-lookup"><span data-stu-id="f104b-106">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="f104b-107">(Du kunde göra det tidigare i ditt Cloud Partner Portal CPP-konto.</span><span class="sxs-lookup"><span data-stu-id="f104b-107">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="f104b-108">Nu när du har migrerat till Partnercenter är CPP-kontot skrivskyddat.)</span><span class="sxs-lookup"><span data-stu-id="f104b-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="f104b-109">Tjänstens huvudnamn är synonymt med Azure AD-programmet.</span><span class="sxs-lookup"><span data-stu-id="f104b-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="f104b-110">Lägga till ett Azure AD-program (tjänstens huvudnamn)</span><span class="sxs-lookup"><span data-stu-id="f104b-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="f104b-111">På instrumentpanelen i Partnercenter väljer **du Inställningar** och sedan Inställningar **för utvecklare.**</span><span class="sxs-lookup"><span data-stu-id="f104b-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="f104b-112">Välj **Användare** och sedan Lägg **till Azure AD-program.**</span><span class="sxs-lookup"><span data-stu-id="f104b-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="f104b-113">Välj ett befintligt Azure AD-program eller skapa ett nytt.</span><span class="sxs-lookup"><span data-stu-id="f104b-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="f104b-114">Om du skapar ett nytt Azure AD-program ska du inkludera följande information:</span><span class="sxs-lookup"><span data-stu-id="f104b-114">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="f104b-115">**Svars-URL:** Den URL där användare kan logga in för att använda ditt Azure AD-program.</span><span class="sxs-lookup"><span data-stu-id="f104b-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="f104b-116">**App-ID-URI:** En logisk identifierare för Azure AD-programmet som visas när den skickar en begäran om enkel inloggning till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f104b-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="f104b-117">**Säkerhetsroller:** Rollhanteraren **(samma** som rollen Ägare i CPP) och **Utvecklare** (samma som rollen Deltagare i CPP) gäller för Commercial Marketplace-programmet i Partnercenter och kan associeras med det här Azure AD-programmet.</span><span class="sxs-lookup"><span data-stu-id="f104b-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="f104b-118">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="f104b-118">Next steps</span></span>

- [<span data-ttu-id="f104b-119">Översikt över den kommersiella marknadsplatsen i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="f104b-119">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)