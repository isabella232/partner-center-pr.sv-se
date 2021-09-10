---
title: Hitta klientorganisations-ID, domännamn, användarobjekt-ID
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Lär dig hur du hittar ID:n i Azure Portal – en organisations Azure AD-klientorganisations-ID, domännamn eller specifikt användarobjekt-ID. Vissa uppgifter behöver den här informationen.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: db730436e88118c24aa966c1023ffeeadd20548a
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960543"
---
# <a name="locate-important-ids-for-a-user"></a>Hitta viktiga ANVÄNDAR-ID:er för en användare

**Lämpliga roller:** Global administratör

Den här artikeln beskriver hur du använder [Azure Portal](https://portal.azure.com/) för att hitta följande information för en användare:

- Klient-ID Microsoft Azure Active Directory (Azure AD) för användarens organisation eller företag

- Det primära domännamnet för den organisation eller det företag som är associerat med Azure AD-klientorganisationen

- Användarobjektets ID

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Hitta Microsoft Azure AD klientorganisations-ID och primärt domännamn

Följ dessa steg för att hitta Azure AD-klientorganisations-ID:t eller det primära domännamnet i Azure Portal. (Om du vill hitta ett klient-ID programmässigt kan du se [Hitta klientorganisations-ID med PowerShell eller CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)

> [!NOTE]
> Klientorganisations-ID:t kan kallas olika namn i olika program eller resurser. Till exempel kan klient-ID kallas katalog-ID, Azure Active Directory (Azure AD)-klient, Microsoft-ID eller för vissa rapporter, även *tenantguid*.

1. Logga in på [Azure-portalen](https://portal.azure.com/).

2. Välj **Azure Active Directory** på menyn.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Visar Azure Portal du väljer Azure Active Directory alternativet i menyn.":::

3. En Azure Active Directory **översiktssida** visas. Leta reda på Id för Azure AD-klient eller primärt domännamn genom att leta efter fältet **Klientorganisations-ID** och **fältet Primär** domän. Dessa fält visas i avsnittet Klientinformation.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Visar översiktssidan med två markerade fält, klientorganisations-ID och primärt domännamn.":::

4. Du hittar klientorganisations-ID:t i Azure Portal på några andra sätt. Välj **Azure Active Directory** på menyn. Leta sedan upp **avsnittet** Hantera på menyn och välj **Egenskaper.**

   Sidan Egenskaper visar även användarens associerade klientorganisations-ID.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Visar sidan Egenskaper med markerat fält för klientorganisations-ID.":::

## <a name="find-the-user-object-id"></a>Hitta användarobjektets ID

Att bara hitta domännamnet och klientorganisations-ID:t kanske inte alltid räcker. Du kan också behöva hitta det specifika objekt-ID som tilldelats en användare. Följ dessa steg för att hitta en användares objekt-ID i Azure Portal:

1. Logga in på [Azure-portalen](https://portal.azure.com/).

2. Välj **Azure Active Directory** på menyn.

3. Leta upp **avsnittet** Hantera på menyn och välj sedan **Användare.**

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Visar Azure Active Directory meny med markerat alternativ Användare.":::

4. På sidan Användare skriver du in användarens namn i sökrutan.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Visar sidan Användare med sökruta för att söka efter en viss användare.":::

5. Välj användarens namn där det visas i listan.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Visar sidan Användare som visar en rad för den sökte användaren.":::

6. Leta upp avsnittet Identitet på användarens profilsida. Fältet Objekt-ID visas här med användarens unika objekt-ID.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Visar sidan Användarprofil med avsnittet Identitet och ett markerat fält för Objekt-ID.":::

## <a name="next-steps"></a>Nästa steg

- [Hitta ditt klientorganisations-ID programmatiskt med PowerShell eller CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Läs mer om användarprofiler i Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Ta reda på hur partner kan se eller exportera kundinformation i Partnercenter](see-your-customer-list.md)

