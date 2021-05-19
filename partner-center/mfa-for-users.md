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
ms.openlocfilehash: 5173526d0f65623311d5cd3a1061e8b9e93e9bb9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151635"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="80754-103">Ge användarna multifaktorautentisering</span><span class="sxs-lookup"><span data-stu-id="80754-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="80754-104">**Lämpliga roller:** Global administratör</span><span class="sxs-lookup"><span data-stu-id="80754-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="80754-105">Större sekretessskydd och säkerhet är bland våra högsta prioriteter.</span><span class="sxs-lookup"><span data-stu-id="80754-105">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="80754-106">Vi vet att det bästa försvaret är att förebygga och att vi bara är lika starka som vår svagaste länk.</span><span class="sxs-lookup"><span data-stu-id="80754-106">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="80754-107">Därför behöver vi att alla i vårt ekosystem agerar och ser till att rätt säkerhetsskydd finns på plats.</span><span class="sxs-lookup"><span data-stu-id="80754-107">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="80754-108">Vi rekommenderar starkt att alla partner aktiverar multifaktorautentisering (MFA) för sina användare i partnerklientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="80754-108">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="80754-109">Lägga till multifaktorautentisering för dina användare</span><span class="sxs-lookup"><span data-stu-id="80754-109">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="80754-110">Du måste vara global administratör för ditt företag för att slutföra den här uppgiften.</span><span class="sxs-lookup"><span data-stu-id="80754-110">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="80754-111">Det är enklast att aktivera MFA för dina användare när du lägger till dem i din Azure AD-klientorganisation.</span><span class="sxs-lookup"><span data-stu-id="80754-111">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="80754-112">Logga in [på Azure Portal](https://portal.azure.com) och gå sedan till **Användarhantering.**</span><span class="sxs-lookup"><span data-stu-id="80754-112">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="80754-113">Välj **Multi-Factor Authentication**.</span><span class="sxs-lookup"><span data-stu-id="80754-113">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="80754-114">Välj den användare som du vill aktivera och välj sedan **Aktivera.**</span><span class="sxs-lookup"><span data-stu-id="80754-114">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="80754-115">Detta aktiverar MFA för den här användaren.</span><span class="sxs-lookup"><span data-stu-id="80754-115">This will enable MFA for this user.</span></span> <span data-ttu-id="80754-116">Aktiverat innebär att användaren uppmanas att konfigurera sin MFA-verifiering när de loggar in för första gången.</span><span class="sxs-lookup"><span data-stu-id="80754-116">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="80754-117">Därefter uppmanas de vid inloggningen att ange en kod som skickas till dem antingen via e-post eller SMS (beroende på vilket de har ställt in).</span><span class="sxs-lookup"><span data-stu-id="80754-117">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Ange hur du ska verifiera":::

>[!NOTE]
><span data-ttu-id="80754-119">Du kan **tvinga** användarna att använda MFA genom att följa samma steg som ovan och välja **Framtvinga.**</span><span class="sxs-lookup"><span data-stu-id="80754-119">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="80754-120">Mer information finns i [Aktivera Azure Multi-Factor Authentication per användare för att skydda inloggningshändelser.](/azure/active-directory/authentication/howto-mfa-userstates)</span><span class="sxs-lookup"><span data-stu-id="80754-120">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="80754-121">Alla användare börjar med **Inaktiverad**.</span><span class="sxs-lookup"><span data-stu-id="80754-121">All users start out **Disabled**.</span></span> <span data-ttu-id="80754-122">När du registrerar användare i per användare Azure Active Directory Multi-Factor Authentication ändras deras tillstånd till **Aktiverad.**</span><span class="sxs-lookup"><span data-stu-id="80754-122">When you enroll users in per-user Azure Active Directory Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="80754-123">När aktiverat användare loggar in och slutför registreringsprocessen ändras deras tillstånd till **Framtvingad**.</span><span class="sxs-lookup"><span data-stu-id="80754-123">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="80754-124">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="80754-124">Next steps</span></span>

- [<span data-ttu-id="80754-125">Tilldela roller och behörigheter till användare</span><span class="sxs-lookup"><span data-stu-id="80754-125">Assign roles and permissions to users</span></span>](permissions-overview.md)