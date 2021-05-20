---
title: Länka ditt arbetskonto för att få åtkomst till Partnercenter
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Skapa ett arbetskonto som länkar ditt företag till ditt Partnercenter-konto. Detta gör att anställda på ditt företag kan komma åt Partnercenter.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: a06a38ef9d96b4c2a1e95328d510eb2fd71ff0e3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149850"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a><span data-ttu-id="fa417-104">Skapa ett arbetskonto som länkar ditt företag till ditt Partnercenter-konto</span><span class="sxs-lookup"><span data-stu-id="fa417-104">Create a work account that links your company to your Partner Center account</span></span>

<span data-ttu-id="fa417-105">**Lämpliga roller:** Globala | Administratör för användarhantering</span><span class="sxs-lookup"><span data-stu-id="fa417-105">**Appropriate roles**: Global admin | User management admin</span></span>

## <a name="why-you-need-a-work-account"></a><span data-ttu-id="fa417-106">Varför du behöver ett arbetskonto</span><span class="sxs-lookup"><span data-stu-id="fa417-106">Why you need a work account</span></span>

<span data-ttu-id="fa417-107">Microsoft kräver att du länkar företagets arbetskonto till ditt nya Partnercenter-konto.</span><span class="sxs-lookup"><span data-stu-id="fa417-107">Microsoft requires you to link your company's work account to your new Partner Center account.</span></span> <span data-ttu-id="fa417-108">Med länken kan dina kontoanvändare logga in på Partnercenter med sina användarnamn och lösenord för arbetskontot.</span><span class="sxs-lookup"><span data-stu-id="fa417-108">The link enables your account users to sign in to Partner Center with their work account user names and passwords.</span></span>

## <a name="the-work-account-email-address"></a><span data-ttu-id="fa417-109">Arbetskontots e-postadress</span><span class="sxs-lookup"><span data-stu-id="fa417-109">The work account email address</span></span>

<span data-ttu-id="fa417-110">Ditt arbetskonto eller din arbets-e-postadress är den e-postadress som ditt företag har angett.</span><span class="sxs-lookup"><span data-stu-id="fa417-110">Your work account or work email is the email address provided to you by your company.</span></span> <span data-ttu-id="fa417-111">E-postadressen för ett arbetskonto har vanligtvis formatet `you@yourcompany.com` .</span><span class="sxs-lookup"><span data-stu-id="fa417-111">A work account email is usually in the format `you@yourcompany.com`.</span></span> <span data-ttu-id="fa417-112">Personliga e-postadresser som Hotmail, Gmail eller Yahoo fungerar inte som e-post och kan inte användas för ditt Partnercenter-konto.</span><span class="sxs-lookup"><span data-stu-id="fa417-112">Personal email addresses such as Hotmail, Gmail, or Yahoo aren't work email and can't be used for your Partner Center account.</span></span>

<span data-ttu-id="fa417-113">Om du har mer än en giltig e-postadress till arbetet använder du den som är kopplad till företagets huvudkontor i stället för till den regionala avdelningen, till exempel, använd din e-postadress i stället för `contoso.com` `contoso.uk` adressen.</span><span class="sxs-lookup"><span data-stu-id="fa417-113">If you have more than one valid work email address, use the one that is associated to your Corporate Headquarters rather than the regional department, for example, use your `contoso.com` email rather than the `contoso.uk` address.</span></span>

> [!NOTE]  
> <span data-ttu-id="fa417-114">Innan du bestämmer dig för att använda ett befintligt arbetskonto bör du tänka på hur många användare i kontot som måste arbeta i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="fa417-114">Before you decide to use an existing work account, think about how many users in the account will need to work in Partner Center.</span></span> <span data-ttu-id="fa417-115">Om du har användare i kontot som inte behöver arbeta i Partnercenter kan du skapa ett nytt konto för endast de användare som behöver arbeta i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="fa417-115">If you have users in the account who won't need to work in Partner Center, consider creating a new account for only those users who will need to work in the Partner Center.</span></span>

## <a name="not-sure-if-your-company-already-has-a-work-account"></a><span data-ttu-id="fa417-116">Är du osäker på om ditt företag redan har ett arbetskonto?</span><span class="sxs-lookup"><span data-stu-id="fa417-116">Not sure if your company already has a work account?</span></span>

<span data-ttu-id="fa417-117">Om du inte är säker på om ditt företag har ett arbetskonto följer du dessa steg för att kontrollera.</span><span class="sxs-lookup"><span data-stu-id="fa417-117">If you're not sure whether your company has a work account, follow these steps to check.</span></span> <span data-ttu-id="fa417-118">Om du har en aktiv prenumeration på Microsoft Azure eller Office 365 har du redan ett arbetskonto.</span><span class="sxs-lookup"><span data-stu-id="fa417-118">If you have an active subscription to Microsoft Azure or Office 365, you already have a work account.</span></span>

1. <span data-ttu-id="fa417-119">Logga in på [Azure-portalen](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="fa417-119">Sign in to the [Azure portal](https://portal.azure.com).</span></span>

2. <span data-ttu-id="fa417-120">Välj Azure Active Directory på menyn och välj sedan Domännamn.</span><span class="sxs-lookup"><span data-stu-id="fa417-120">Select Azure Active Directory from the menu and then select Domain Names.</span></span>

3. <span data-ttu-id="fa417-121">Om du redan har ett arbetskonto visas domännamnet.</span><span class="sxs-lookup"><span data-stu-id="fa417-121">If you already have a work account, your domain name will be listed.</span></span>

<span data-ttu-id="fa417-122">Om ditt företag inte redan har ett arbetskonto kan du skapa ett under registreringsprocessen.</span><span class="sxs-lookup"><span data-stu-id="fa417-122">If your company doesn't already have a work account, you can create one during the enrollment process.</span></span>

<span data-ttu-id="fa417-123">Diagrammet nedan innehåller steg för flera vanliga scenarier:</span><span class="sxs-lookup"><span data-stu-id="fa417-123">The diagram below provides steps for several typical scenarios:</span></span>

- <span data-ttu-id="fa417-124">avgöra om du har ett arbetskonto</span><span class="sxs-lookup"><span data-stu-id="fa417-124">determine if you have a work account</span></span>
- <span data-ttu-id="fa417-125">bestämma hur du loggar in på ditt arbetskonto</span><span class="sxs-lookup"><span data-stu-id="fa417-125">determine how to sign into your work account</span></span>
- <span data-ttu-id="fa417-126">avgöra om du behöver skapa ett nytt arbetskonto</span><span class="sxs-lookup"><span data-stu-id="fa417-126">determine if you need to create a new work account</span></span>

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Har du ett arbetskonto eller behöver du skapa ett?":::

<span data-ttu-id="fa417-128">Mer information om hur du lägger till domäner i Azure AD finns i [Lägga till eller associera en domän i Azure AD](/azure/active-directory/active-directory-add-domain)</span><span class="sxs-lookup"><span data-stu-id="fa417-128">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="fa417-129">Om Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="fa417-129">About Microsoft Azure</span></span>

<span data-ttu-id="fa417-130">Microsoft Azure är en offentlig molnplattform som företag kan använda för att skapa, distribuera och hantera program i ett globalt nätverk med Microsoft-hanterade datacenter.</span><span class="sxs-lookup"><span data-stu-id="fa417-130">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="fa417-131">Företag använder Azure för att skapa en virtuell IT-infrastruktur med virtuella funktioner, eller tjänster, i stället för fysiska datorer.</span><span class="sxs-lookup"><span data-stu-id="fa417-131">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span>

<span data-ttu-id="fa417-132">När du köper en Azure-prenumeration hyr du i princip ett dedikerat, skyddat utrymme i det offentliga Azure-molnet, inte för mycket från att hyra en våning i en kontorsbyggnad för att inhysa företagets fysiska verksamhet.</span><span class="sxs-lookup"><span data-stu-id="fa417-132">When you purchase an Azure subscription, you're essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company's physical business.</span></span> <span data-ttu-id="fa417-133">Ditt företag är en klientorganisation för kontorsbyggnadsägaren.</span><span class="sxs-lookup"><span data-stu-id="fa417-133">To the office building's owner, your company is a tenant.</span></span>

<span data-ttu-id="fa417-134">Ett Azure-arbetskonto är en dedikerad och isolerad virtuell representation av ditt företag i det offentliga Azure-molnet som skapas åt dig när du prenumererar på en Microsoft-molntjänst som Azure, Microsoft Intune eller Office 365.</span><span class="sxs-lookup"><span data-stu-id="fa417-134">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="fa417-135">Ditt arbetskonto är värd för dina Azure AD-användare och information om dem – deras lösenord, profildata, behörigheter och så vidare.</span><span class="sxs-lookup"><span data-stu-id="fa417-135">Your work account hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="fa417-136">Arbetskontot innehåller också grupper, program och annan information som rör ett företag och dess säkerhet.</span><span class="sxs-lookup"><span data-stu-id="fa417-136">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fa417-137">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="fa417-137">Next steps</span></span>

- [<span data-ttu-id="fa417-138">Hantera ditt Partnercenter-konto</span><span class="sxs-lookup"><span data-stu-id="fa417-138">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="fa417-139">Spåra verifieringsstatus</span><span class="sxs-lookup"><span data-stu-id="fa417-139">Track verification status</span></span>](verification-responses.md)