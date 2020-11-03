---
title: Azure AD-tjänstens huvud namn
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ta reda på hur du lägger till ett huvud namn för tjänsten i Azure AD-klienten. Det innebär att du lägger till ett Azure AD-program (tjänstens huvud namn) i Partner Center.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2020
ms.locfileid: "92531217"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="d4f6a-104">Lägga till ett Azure AD-program (tjänstens huvud namn) i Partner Center</span><span class="sxs-lookup"><span data-stu-id="d4f6a-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="d4f6a-105">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="d4f6a-105">**Applies to**</span></span>

- <span data-ttu-id="d4f6a-106">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="d4f6a-106">Partner Center</span></span>

<span data-ttu-id="d4f6a-107">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="d4f6a-107">**Appropriate roles**</span></span>

- <span data-ttu-id="d4f6a-108">Global administratör</span><span class="sxs-lookup"><span data-stu-id="d4f6a-108">Global admin</span></span>

<span data-ttu-id="d4f6a-109">I programmet för kommersiella marknads platser i Partner Center kan du nu lägga till ett Azure AD-program (tjänstens huvud namn) som en användare i ditt partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="d4f6a-109">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="d4f6a-110">(Du kunde göra det tidigare i din Cloud Partner Portal eller CPP, konto.</span><span class="sxs-lookup"><span data-stu-id="d4f6a-110">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="d4f6a-111">Nu när du har migrerat till Partner Center är kontot CPP skrivskyddat.)</span><span class="sxs-lookup"><span data-stu-id="d4f6a-111">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="d4f6a-112">Tjänstens huvud namn är synonymt med Azure AD-programmet.</span><span class="sxs-lookup"><span data-stu-id="d4f6a-112">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="d4f6a-113">Lägg till ett Azure AD-program (tjänstens huvud namn)</span><span class="sxs-lookup"><span data-stu-id="d4f6a-113">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="d4f6a-114">Välj **Inställningar** på instrument panelen för partner Center och välj sedan inställningar för **utvecklare** .</span><span class="sxs-lookup"><span data-stu-id="d4f6a-114">From the Partner Center dashboard, select **Settings** and then select **Developer settings** .</span></span>

2. <span data-ttu-id="d4f6a-115">Välj **användare** och välj sedan **Lägg till Azure AD-program** .</span><span class="sxs-lookup"><span data-stu-id="d4f6a-115">Select **Users** and then select **Add Azure AD Applications** .</span></span>

3. <span data-ttu-id="d4f6a-116">Välj ett befintligt Azure AD-program eller skapa ett nytt.</span><span class="sxs-lookup"><span data-stu-id="d4f6a-116">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="d4f6a-117">Om du skapar ett nytt Azure AD-program inkluderar du följande information:</span><span class="sxs-lookup"><span data-stu-id="d4f6a-117">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="d4f6a-118">**Svars-URL** : URL: en där användarna kan logga in för att använda ditt Azure AD-program.</span><span class="sxs-lookup"><span data-stu-id="d4f6a-118">**Reply URL** : The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="d4f6a-119">**App-ID-URI** : ett logiskt ID för Azure AD-programmet som presenteras när den skickar en begäran om enkel inloggning till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d4f6a-119">**App ID URI** : A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="d4f6a-120">**Säkerhets roller** : roll **hanteraren** (samma som ägar rollen i cpp) och **utvecklaren** (samma som rollen deltagare i cpp) gäller för programmet för kommersiella marknads platser i Partner Center, och de kan ASSOCIERAs med det här Azure AD-programmet.</span><span class="sxs-lookup"><span data-stu-id="d4f6a-120">**Security roles** : The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="d4f6a-121">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d4f6a-121">Next steps</span></span>

- [<span data-ttu-id="d4f6a-122">Översikt över den kommersiella marknads platsen i Partner Center</span><span class="sxs-lookup"><span data-stu-id="d4f6a-122">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)