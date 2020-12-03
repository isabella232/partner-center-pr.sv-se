---
title: Azure Cost Management av Cloudyn för CSP
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du registrerar Cloudyn-webbappen och använder en hemlig nyckel för den i Partner Center så att du kan använda appen för att spåra användning och kostnader för Azure.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96535004"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="020af-103">Spåra kund Azure-användning och-kostnader med Azure Cost Management-appen för CSP-partner</span><span class="sxs-lookup"><span data-stu-id="020af-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="020af-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="020af-104">**Appropriate roles**</span></span>

- <span data-ttu-id="020af-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="020af-105">Global admin</span></span>
- <span data-ttu-id="020af-106">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="020af-106">Admin agent</span></span>

[<span data-ttu-id="020af-107">Få mer information om Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="020af-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="020af-108">Innan du börjar</span><span class="sxs-lookup"><span data-stu-id="020af-108">Before you begin</span></span>
<span data-ttu-id="020af-109">Innan du kan använda Azure Cost Management kontrollerar du att du uppfyller följande krav:</span><span class="sxs-lookup"><span data-stu-id="020af-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="020af-110">Du är en partner i Cloud Solution Provider-programmet.</span><span class="sxs-lookup"><span data-stu-id="020af-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="020af-111">Du kan skapa en API-webbapp för partner Center.</span><span class="sxs-lookup"><span data-stu-id="020af-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="020af-112">Översikt</span><span class="sxs-lookup"><span data-stu-id="020af-112">Overview</span></span>

<span data-ttu-id="020af-113">Cloudyn är en webbapp som gör att du kan spåra och hantera hur mycket dina kunder använder Azure och kostnaden för den användningen.</span><span class="sxs-lookup"><span data-stu-id="020af-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="020af-114">Du använder det via partner Center API.</span><span class="sxs-lookup"><span data-stu-id="020af-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="020af-115">Registrera din webbapp i Partner Center</span><span class="sxs-lookup"><span data-stu-id="020af-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="020af-116">När du registrerar en Azure Active Directory webbapp i Partner Center ger du åtkomst till Partner Center-API: et.</span><span class="sxs-lookup"><span data-stu-id="020af-116">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="020af-117">Logga in på [partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) med ett [globalt administratörs-eller administratörs agent konto](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="020af-117">Sign into [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="020af-118">Från **partner Center** väljer du **konto inställningar** &gt; **[app Management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="020af-118">From **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="020af-119">I avsnittet **webbapp** klickar du på **Lägg till ny webbapp**.</span><span class="sxs-lookup"><span data-stu-id="020af-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="020af-120">**Obs**: om du tidigare har skapat en webbapp kan du hoppa över steg 3.</span><span class="sxs-lookup"><span data-stu-id="020af-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="020af-121">Kopiera och spara **handels-ID-** GUID och GUID för **app-ID** för din webbapp.</span><span class="sxs-lookup"><span data-stu-id="020af-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="020af-122">Du behöver båda ID: na för att använda den 30 dagars kostnads fria utvärderings versionen av Azure Cost Management-appen.</span><span class="sxs-lookup"><span data-stu-id="020af-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="020af-123">Lägg till en hemlig nyckel i appen</span><span class="sxs-lookup"><span data-stu-id="020af-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="020af-124">I list rutan bredvid knappen **Lägg till nyckel** väljer du varaktigheten 1 eller 2 år.</span><span class="sxs-lookup"><span data-stu-id="020af-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="020af-125">Klicka på **Lägg till nyckel**.</span><span class="sxs-lookup"><span data-stu-id="020af-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="020af-126">Kopiera och spara värdet för den hemliga nyckeln.</span><span class="sxs-lookup"><span data-stu-id="020af-126">Copy and save the secret key value.</span></span> <span data-ttu-id="020af-127">Du behöver detta för den 30-dagars kostnads fria utvärderings versionen.</span><span class="sxs-lookup"><span data-stu-id="020af-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="020af-128">Programmets hemliga nycklar liknar lösen ord med längre förfallo datum.</span><span class="sxs-lookup"><span data-stu-id="020af-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="020af-129">Spara nyckelvärdet på en säker plats för framtida användning.</span><span class="sxs-lookup"><span data-stu-id="020af-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="020af-130">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="020af-130">Next steps</span></span>
<span data-ttu-id="020af-131">Starta en [30-dagars kostnads fri utvärderings version](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="020af-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="020af-132">Du behöver följande information för att starta utvärderings versionen:</span><span class="sxs-lookup"><span data-stu-id="020af-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="020af-133">Inloggnings uppgifter för partner Center</span><span class="sxs-lookup"><span data-stu-id="020af-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="020af-134">GUID för handels-ID</span><span class="sxs-lookup"><span data-stu-id="020af-134">Commerce ID GUID</span></span>
- <span data-ttu-id="020af-135">GUID för app-ID</span><span class="sxs-lookup"><span data-stu-id="020af-135">App ID GUID</span></span>
- <span data-ttu-id="020af-136">Nyckel värde för program hemligt</span><span class="sxs-lookup"><span data-stu-id="020af-136">Application secret key value</span></span>
