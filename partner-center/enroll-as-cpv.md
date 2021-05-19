---
title: Registrera dig som Kontrollpanelen leverantör
description: Lär dig hur du registrerar dig som en Kontrollpanelen Vendor (CPV) i Partner Center så att du bättre kan integrera CSP-partnersystem med Partner Center-API:er.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: edc0ea8f0fda58f23cbce82bc7023a3277517cc3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147147"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="e0cb8-103">Registrera dig som en Kontrollpanelen leverantör för att integrera CSP-partnersystem med Partner Center-API:er</span><span class="sxs-lookup"><span data-stu-id="e0cb8-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="e0cb8-104">**Lämpliga roller:** Global administratör</span><span class="sxs-lookup"><span data-stu-id="e0cb8-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="e0cb8-105">En Kontrollpanelen Vendor (CPV) är en oberoende programvaruleverantör som utvecklar program för användning av Molnlösningsleverantör-partner (CSP) så att de kan integrera sina system med Partner Center-API:er.</span><span class="sxs-lookup"><span data-stu-id="e0cb8-105">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="e0cb8-106">En Kontrollpanelen leverantör är inte en CSP-partner med direkt åtkomst till Partner Center-instrumentpanelen eller Partnercenter-API:er.</span><span class="sxs-lookup"><span data-stu-id="e0cb8-106">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="e0cb8-107">Oavsett om du är en aktuell Kontrollpanelen Vendor (CPV) eller en ny CPV som vill arbeta med Microsoft-partner kräver Microsoft nu att du registrerar dig i PartnerCenter för att registrera dina program och stödja Molnlösningsleverantör partner.</span><span class="sxs-lookup"><span data-stu-id="e0cb8-107">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="e0cb8-108">Om du vill skapa ett konto kan en CPV-partner antingen använda en befintlig CSP-partnerklientorganisation eller en befintlig CPV-klient eller skapa en ny klient som en del av registreringsprocessen.</span><span class="sxs-lookup"><span data-stu-id="e0cb8-108">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="e0cb8-109">Om CPV-partnern väljer att använda den befintliga CSP-klienten måste de skapa separata program för flera innehavare och registrera dem i Partnercenter för CPV-aktiviteter.</span><span class="sxs-lookup"><span data-stu-id="e0cb8-109">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="e0cb8-110">Ett program kan inte registreras som både ett CSP- och CPV-program.</span><span class="sxs-lookup"><span data-stu-id="e0cb8-110">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="e0cb8-111">När du har registrerat dig i Partnercenter och registrerat dina program har du åtkomst till Partner Center-API:erna.</span><span class="sxs-lookup"><span data-stu-id="e0cb8-111">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="e0cb8-112">Kontakta Microsoft via en Microsoft Support om du behöver ett sandbox-konto.</span><span class="sxs-lookup"><span data-stu-id="e0cb8-112">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="e0cb8-113">Om du redan har ett sandbox-konto kan du fortsätta att använda det.</span><span class="sxs-lookup"><span data-stu-id="e0cb8-113">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="e0cb8-114">Du behöver ingen ny sandbox-miljö</span><span class="sxs-lookup"><span data-stu-id="e0cb8-114">You won't need a new sandbox</span></span>

<span data-ttu-id="e0cb8-115">Granska [Microsoft Kontrollpanelen vendor-avtalet](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="e0cb8-115">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="e0cb8-116">Arbeta i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="e0cb8-116">Working in Partner Center</span></span>

<span data-ttu-id="e0cb8-117">När du har registrerat dig för CPV-upplevelsen i Partnercenter och godkänt CPV-avtalet kan du:</span><span class="sxs-lookup"><span data-stu-id="e0cb8-117">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="e0cb8-118">Hantera program för flera innehavare (lägg till program i Azure Portal, registrera och avregistrera program i Partnercenter).</span><span class="sxs-lookup"><span data-stu-id="e0cb8-118">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="e0cb8-119">CPV:er måste registrera sina program i Partnercenter för att få behörighet för Partner Center-API:er.</span><span class="sxs-lookup"><span data-stu-id="e0cb8-119">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="e0cb8-120">Att lägga till program i Azure Portal auktoriserar inte CPV-program för Partner Center-API:er.</span><span class="sxs-lookup"><span data-stu-id="e0cb8-120">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="e0cb8-121">Visa och hantera din CPV-profil</span><span class="sxs-lookup"><span data-stu-id="e0cb8-121">View and manage your CPV profile</span></span> 

- <span data-ttu-id="e0cb8-122">Visa och hantera användare som behöver åtkomst till CPV-funktioner.</span><span class="sxs-lookup"><span data-stu-id="e0cb8-122">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="e0cb8-123">Global administratör är den enda roll som en CPV kan ha.</span><span class="sxs-lookup"><span data-stu-id="e0cb8-123">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e0cb8-124">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="e0cb8-124">Next steps</span></span>

<span data-ttu-id="e0cb8-125">-[Lägga till ytterligare klienter till ditt Partnercenter-konto](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="e0cb8-125">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>