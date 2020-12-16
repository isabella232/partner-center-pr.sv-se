---
title: Ge användarna multifaktorautentisering
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur du ställer in dina anställda med MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 355258fd20f867052fa8598e688630005262bb16
ms.sourcegitcommit: ab2ca3c5990b7f920df4ecb9c611d5b1046ec111
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/16/2020
ms.locfileid: "97579982"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="5ce4d-103">Ge användarna multifaktorautentisering</span><span class="sxs-lookup"><span data-stu-id="5ce4d-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="5ce4d-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="5ce4d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="5ce4d-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="5ce4d-105">Global admin</span></span>

<span data-ttu-id="5ce4d-106">Större Sekretess skydd och säkerhet är bland våra främsta prioriteringar.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="5ce4d-107">Vi vet att det bästa skyddet är förebyggande och att vi bara är lika starka som vår svagaste länk.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="5ce4d-108">Därför behöver vi alla i vårt eko system för att agera och se till att lämpliga säkerhets skydd är på plats.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="5ce4d-109">Vi rekommenderar starkt att alla partners aktiverar Multi-Factor Authentication (MFA) för sina användare i sin partner klient organisation.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="5ce4d-110">Lägg till Multi-Factor Authentication för dina användare</span><span class="sxs-lookup"><span data-stu-id="5ce4d-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="5ce4d-111">Du måste vara den globala administratören för ditt företag för att slutföra den här uppgiften.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="5ce4d-112">Det är enklast att aktivera MFA för dina användare när du lägger till dem i din Azure AD-klient.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="5ce4d-113">Logga in på [Azure Portal](https://portal.azure.com) och gå sedan till **användar hantering**.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="5ce4d-114">Välj **Multi-Factor Authentication**.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="5ce4d-115">Välj den användare som du vill aktivera och välj sedan **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="5ce4d-116">Detta aktiverar MFA för den här användaren.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-116">This will enable MFA for this user.</span></span> <span data-ttu-id="5ce4d-117">Aktive rad innebär att användaren uppmanas att ställa in sin MFA-verifiering när de loggar in för första gången.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="5ce4d-118">Därefter uppmanas han eller hon att ange en kod som skickas till dem antingen via e-post eller SMS (beroende på vilka de har ställt in).</span><span class="sxs-lookup"><span data-stu-id="5ce4d-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Ange hur du vill verifiera":::

>[!NOTE]
><span data-ttu-id="5ce4d-120">Du kan **tvinga** dina användare att använda MFA genom att använda samma steg som ovan och välja **tvinga**.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="5ce4d-121">Läs mer i [Aktivera Azure-Multi-Factor Authentication per användare för att skydda inloggnings händelser](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="5ce4d-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="5ce4d-122">Alla användare börjar vara **inaktiverade**.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-122">All users start out **Disabled**.</span></span> <span data-ttu-id="5ce4d-123">När du registrerar användare i Azure-Multi-Factor Authentication per användare, ändras deras status till **aktive rad**.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="5ce4d-124">När aktiverade användare loggar in och slutför registrerings processen ändras deras status till **tvingande**.</span><span class="sxs-lookup"><span data-stu-id="5ce4d-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="5ce4d-125">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="5ce4d-125">Next steps</span></span>

- [<span data-ttu-id="5ce4d-126">Tilldela roller och behörigheter till användare</span><span class="sxs-lookup"><span data-stu-id="5ce4d-126">Assign roles and permissions to users</span></span>](permissions-overview.md)

