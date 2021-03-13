---
title: Överförings berättigande – rikt linjer för överföring av en prenumeration mellan fakturerings konton, Azure Marketplace
description: Rikt linjer för kommersiella kontroller innan du överför en prenumeration mellan fakturerings konton i Azure Portal.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412564"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="3a617-103">Överför berättigande för en prenumeration mellan fakturerings konton</span><span class="sxs-lookup"><span data-stu-id="3a617-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="3a617-104">Du kan [överföra en prenumeration](/azure/cost-management-billing/understand/subscription-transfer) från ett fakturerings konto till ett annat i fakturerings avsnittet i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="3a617-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="3a617-105">Före en överföring genomsöks prenumerationen efter produkter från tredje part.</span><span class="sxs-lookup"><span data-stu-id="3a617-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="3a617-106">Överföringen tillåts bara om *alla* produkter har rensats för överföring (se [kriterierna](#criteria-for-transfer-approval-or-denial) nedan).</span><span class="sxs-lookup"><span data-stu-id="3a617-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="3a617-107">Systemet genererar relevanta fel meddelanden för de appar som inte kunde rensas för att hjälpa dig att fastställa nästa steg.</span><span class="sxs-lookup"><span data-stu-id="3a617-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="3a617-108">Den här artikeln gäller inte för SaaS-erbjudanden eftersom SaaS-resurser är kopplade till en klient, inte en prenumeration.</span><span class="sxs-lookup"><span data-stu-id="3a617-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="3a617-109">SaaS-resurser kan överföras från ett fakturerings konto till ett annat, men detta görs per resurs och av Azure-support som en support förfrågan.</span><span class="sxs-lookup"><span data-stu-id="3a617-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="3a617-110">Villkor för godkännande eller avslag av överföring</span><span class="sxs-lookup"><span data-stu-id="3a617-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="3a617-111">Du kan inte överföra en prenumeration om någon av dess appar från tredje part uppfyller något av följande kriterier:</span><span class="sxs-lookup"><span data-stu-id="3a617-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="3a617-112">Mål kontot är kommersiellt och appen är inte valbar för att säljas via partner.</span><span class="sxs-lookup"><span data-stu-id="3a617-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="3a617-113">Appen är valbar för utvalda partner och mål kontot finns inte i listan över tillåtna.</span><span class="sxs-lookup"><span data-stu-id="3a617-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="3a617-114">Erbjudandet var ett för hands erbjudande tidigare för valda prenumerationer eller var ett privat erbjudande och prenumerationen är inte längre i listan över tillåtna.</span><span class="sxs-lookup"><span data-stu-id="3a617-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="3a617-115">Det nya fakturerings kontot finns i en annan region än där erbjudandet säljs och erbjudandet är inte att säljas i den regionen.</span><span class="sxs-lookup"><span data-stu-id="3a617-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="3a617-116">En blockerad överföring fortsätter att gälla tills du tar bort resursen från prenumerationen. därefter kan du prova överföringen igen.</span><span class="sxs-lookup"><span data-stu-id="3a617-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3a617-117">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="3a617-117">Next steps</span></span>

[<span data-ttu-id="3a617-118">Få support för Microsoft AppSource och Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="3a617-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

