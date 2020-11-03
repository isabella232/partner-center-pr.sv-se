---
title: Hitta klient-ID, domän namn, användar objekt-ID
ms.topic: how-to
ms.date: 09/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Lär dig hitta ID: n i Azure Portal-en organisations Azure AD-klient-ID, domän namn eller ett särskilt användar objekt-ID. Vissa uppgifter behöver den här informationen.'
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4a3695079a9d5b0b3c66b7c2eda52a31888a6660
ms.sourcegitcommit: 3158b0de261539694e37e433c763afa4067e36fb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/17/2020
ms.locfileid: "92531461"
---
# <a name="locate-important-ids-for-a-user"></a>Hitta viktiga ID: n för en användare

Den här artikeln beskriver hur du använder [Azure Portal](https://portal.azure.com/) för att hitta följande information för en användare:

- Microsoft Azure Active Directory (Azure AD) klient-ID för användarens organisation eller företag

- Det primära domän namnet för den organisation eller det företag som är associerat med Azure AD-klienten

- Användar objektets ID

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Hitta Microsoft Azure AD klient-ID och primärt domän namn

Följ de här stegen för att hitta Azure AD-klient-ID: t eller det primära domän namnet inom Azure Portal.

> [!NOTE]
> Klient-ID: t kan anropas med olika namn i olika program eller resurser. Klient-ID: t kan till exempel kallas katalog-ID, Azure Active Directory (Azure AD)-klient, Microsoft-ID eller för vissa rapporter, även *tenantguid* .

1. Logga in på [Azure-portalen](https://portal.azure.com/).

2. Välj **Azure Active Directory** på menyn.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Visar Azure Portal att välja alternativet Azure Active Directory på menyn.":::

3. Sidan **Översikt över** Azure Active Directory visas. Du hittar Azure AD-klient-ID: t eller det primära domän namnet genom att leta efter **klient-ID-** fältet och det **primära domän** fältet. Dessa fält visas i avsnittet klient information.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Visar Azure Portal att välja alternativet Azure Active Directory på menyn.":::

4. Du kan hitta klient-ID: t i Azure Portal på några andra sätt. Välj **Azure Active Directory** på menyn. Leta sedan upp avsnittet **Hantera** på menyn och välj **Egenskaper** .

   På sidan Egenskaper visas även användarens associerade klient-ID.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Visar Azure Portal att välja alternativet Azure Active Directory på menyn.":::

## <a name="find-the-user-object-id"></a>Hitta användar objektets ID

Det är inte alltid tillräckligt med att hitta domän namnet och klient-ID: t. Du kan också behöva hitta det objekt-ID som tilldelats till en användare. Följ de här stegen för att hitta en användares objekt-ID i Azure Portal:

1. Logga in på [Azure-portalen](https://portal.azure.com/).

2. Välj **Azure Active Directory** på menyn.

3. Leta upp avsnittet **Hantera** på menyn och välj sedan **användare** .

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Visar Azure Portal att välja alternativet Azure Active Directory på menyn.":::

4. På sidan användare anger du användarens namn i sökrutan.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Visar Azure Portal att välja alternativet Azure Active Directory på menyn.":::

5. Välj användarens namn där det visas i listan.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Visar Azure Portal att välja alternativet Azure Active Directory på menyn.":::

6. Leta upp avsnittet identitet på användarens profil sida. Fältet objekt-ID visas här med användarens unika objekt-ID.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Visar Azure Portal att välja alternativet Azure Active Directory på menyn.":::

## <a name="next-steps"></a>Nästa steg

- [Lär dig mer om användar profiler i Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Ta reda på hur partner kan se eller exportera kund information i Partner Center](see-your-customer-list.md)