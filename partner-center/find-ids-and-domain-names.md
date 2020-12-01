---
title: Hitta klient-ID, domän namn, användar objekt-ID
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Lär dig hitta ID: n i Azure Portal-en organisations Azure AD-klient-ID, domän namn eller ett särskilt användar objekt-ID. Vissa uppgifter behöver den här informationen.'
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: cb0325aae30fe57a4be2be3e37bca1ee6aa1eab8
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439236"
---
# <a name="locate-important-ids-for-a-user"></a>Hitta viktiga ID: n för en användare

Den här artikeln beskriver hur du använder [Azure Portal](https://portal.azure.com/) för att hitta följande information för en användare:

- Microsoft Azure Active Directory (Azure AD) klient-ID för användarens organisation eller företag

- Det primära domän namnet för den organisation eller det företag som är associerat med Azure AD-klienten

- Användar objektets ID

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Hitta Microsoft Azure AD klient-ID och primärt domän namn

Följ de här stegen för att hitta Azure AD-klient-ID: t eller det primära domän namnet inom Azure Portal. (Om du vill hitta ett klient-ID program mässigt kan du läsa [hitta klient-ID med PowerShell eller CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)

> [!NOTE]
> Klient-ID: t kan anropas med olika namn i olika program eller resurser. Klient-ID: t kan till exempel kallas katalog-ID, Azure Active Directory (Azure AD)-klient, Microsoft-ID eller för vissa rapporter, även *tenantguid*.

1. Logga in på [Azure-portalen](https://portal.azure.com/).

2. Välj **Azure Active Directory** på menyn.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Visar Azure Portal att välja alternativet Azure Active Directory på menyn.":::

3. Sidan **Översikt över** Azure Active Directory visas. Du hittar Azure AD-klient-ID: t eller det primära domän namnet genom att leta efter **klient-ID-** fältet och det **primära domän** fältet. Dessa fält visas i avsnittet klient information.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Visar översikts sidan med två markerade fält, klient-ID och primärt domän namn.":::

4. Du kan hitta klient-ID: t i Azure Portal på några andra sätt. Välj **Azure Active Directory** på menyn. Leta sedan upp avsnittet **Hantera** på menyn och välj **Egenskaper**.

   På sidan Egenskaper visas även användarens associerade klient-ID.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Visar sidan Egenskaper med det markerade klient-ID-fältet.":::

## <a name="find-the-user-object-id"></a>Hitta användar objektets ID

Det är inte alltid tillräckligt med att hitta domän namnet och klient-ID: t. Du kan också behöva hitta det objekt-ID som tilldelats till en användare. Följ de här stegen för att hitta en användares objekt-ID i Azure Portal:

1. Logga in på [Azure-portalen](https://portal.azure.com/).

2. Välj **Azure Active Directory** på menyn.

3. Leta upp avsnittet **Hantera** på menyn och välj sedan **användare**.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Visar Azure Active Directory menyn med alternativet markerat, användare.":::

4. På sidan användare anger du användarens namn i sökrutan.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Visar sidan användare med sökrutan för att söka efter en speciell användare.":::

5. Välj användarens namn där det visas i listan.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Visar användar sidan som visar en rad för den genomsökta användaren.":::

6. Leta upp avsnittet identitet på användarens profil sida. Fältet objekt-ID visas här med användarens unika objekt-ID.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Visar sidan användar profil med avsnittet identitet och ett markerat fält för objekt-ID.":::

## <a name="next-steps"></a>Nästa steg

- [Hitta ditt klient-ID program mässigt med PowerShell eller CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Lär dig mer om användar profiler i Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Ta reda på hur partner kan se eller exportera kund information i Partner Center](see-your-customer-list.md)

