---
title: Registrera dig som en kontroll panels leverantör
description: 'Lär dig hur du registrerar sig som en kontroll panel leverantör (CPV) i Partner Center så att du bättre kan integrera CSP-partnersystem med API: er för partner Center.'
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: 5fd2267d53641fe4a0b6181217a35f0470e5bbe5
ms.sourcegitcommit: 7681c6fc51e78cba106c46a52f6bb27e1a5c1c6b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "98560518"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="24d43-103">Registrera dig som en kontroll panels leverantör för att integrera CSP-partnersystem med API: er för partner Center</span><span class="sxs-lookup"><span data-stu-id="24d43-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="24d43-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="24d43-104">**Appropriate roles**</span></span>

- <span data-ttu-id="24d43-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="24d43-105">Global admin</span></span>

<span data-ttu-id="24d43-106">En kontroll panel leverantör (CPV) är en oberoende program varu leverantör som utvecklar program som kan användas av leverantörer av moln lösningar (CSP), så att de kan integrera sina system med API: er för partner Center.</span><span class="sxs-lookup"><span data-stu-id="24d43-106">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="24d43-107">En kontroll panel leverantör är ingen CSP-partner med direkt åtkomst till Partner Center-instrumentpanelen eller API: er för partner Center.</span><span class="sxs-lookup"><span data-stu-id="24d43-107">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="24d43-108">Oavsett om du är en aktuell kontroll panels leverantör (CPV) eller en ny CPV som vill arbeta med Microsoft-partner, kräver Microsoft nu att du anmäler dig i Partner Center för att kunna registrera dina program och få support leverantörer till partner leverantörer av moln lösningar.</span><span class="sxs-lookup"><span data-stu-id="24d43-108">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="24d43-109">Om du vill skapa ett konto kan en CPV-partner antingen använda en befintlig CSP-partners klient organisation eller befintlig CPV-klient eller skapa en ny klient som en del av onboarding-processen.</span><span class="sxs-lookup"><span data-stu-id="24d43-109">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="24d43-110">Om CPV-partnern väljer att använda den befintliga CSP-klienten måste de skapa separata program för flera klienter och registrera dem i Partner Center för CPV-aktiviteter.</span><span class="sxs-lookup"><span data-stu-id="24d43-110">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="24d43-111">Det går inte att registrera ett program som både CSP-och CPV-program.</span><span class="sxs-lookup"><span data-stu-id="24d43-111">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="24d43-112">När du har registrerat dig i Partner Center och registrerat dina program har du åtkomst till Partner Center-API: erna.</span><span class="sxs-lookup"><span data-stu-id="24d43-112">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="24d43-113">Kontakta Microsoft via en Microsoft Support begäran om du behöver ett begränsat konto.</span><span class="sxs-lookup"><span data-stu-id="24d43-113">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="24d43-114">Om du redan har ett begränsat konto kan du fortsätta att använda det.</span><span class="sxs-lookup"><span data-stu-id="24d43-114">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="24d43-115">Du behöver inte ett nytt begränsat läge</span><span class="sxs-lookup"><span data-stu-id="24d43-115">You won't need a new sandbox</span></span>

<span data-ttu-id="24d43-116">Granska [Microsoft kontroll panelens leverantörs avtal](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="24d43-116">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="24d43-117">Arbeta i Partner Center</span><span class="sxs-lookup"><span data-stu-id="24d43-117">Working in Partner Center</span></span>

<span data-ttu-id="24d43-118">När du har registrerat dig i Partner Center CPV-upplevelsen och godkänt CPV-avtalet kan du:</span><span class="sxs-lookup"><span data-stu-id="24d43-118">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="24d43-119">Hantera program med flera klienter (Lägg till program i Azure Portal, registrera och avregistrera program i Partner Center).</span><span class="sxs-lookup"><span data-stu-id="24d43-119">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="24d43-120">CPVs måste registrera sina program i Partner Center för att få behörighet för API: er för partner Center.</span><span class="sxs-lookup"><span data-stu-id="24d43-120">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="24d43-121">Att lägga till program till enbart Azure Portal tillåter inte CPV-program för API: er för partner Center.</span><span class="sxs-lookup"><span data-stu-id="24d43-121">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="24d43-122">Visa och hantera din CPV-profil</span><span class="sxs-lookup"><span data-stu-id="24d43-122">View and manage your CPV profile</span></span> 

- <span data-ttu-id="24d43-123">Visa och hantera dina användare som behöver åtkomst till CPV-funktioner.</span><span class="sxs-lookup"><span data-stu-id="24d43-123">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="24d43-124">Global administratör är den enda roll a CPV kan ha.</span><span class="sxs-lookup"><span data-stu-id="24d43-124">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="24d43-125">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="24d43-125">Next steps</span></span>

<span data-ttu-id="24d43-126">-[Lägg till ytterligare klienter till ditt partner Center-konto](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="24d43-126">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>