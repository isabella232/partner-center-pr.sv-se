---
title: Azure AD-tjänstens huvud namn
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ta reda på hur du lägger till ett huvud namn för tjänsten i Azure AD-klienten. Det innebär att du lägger till ett Azure AD-program (tjänstens huvud namn) i Partner Center.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ef5373fd9a606cd25345cbe80a55f28fc1f753f
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028476"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Lägga till ett Azure AD-program (tjänstens huvud namn) i Partner Center

**Lämpliga roller**

- Global administratör

I programmet för kommersiella marknads platser i Partner Center kan du nu lägga till ett Azure AD-program (tjänstens huvud namn) som en användare i ditt partner Center-konto. (Du kunde göra det tidigare i din Cloud Partner Portal eller CPP, konto. Nu när du har migrerat till Partner Center är kontot CPP skrivskyddat.)
 
>[!Note] 
>Tjänstens huvud namn är synonymt med Azure AD-programmet.

## <a name="add-an-azure-ad-application-service-principal"></a>Lägg till ett Azure AD-program (tjänstens huvud namn)

1. Välj **Inställningar** på instrument panelen för partner Center och välj sedan inställningar för **utvecklare**.

2. Välj **användare** och välj sedan **Lägg till Azure AD-program**.

3. Välj ett befintligt Azure AD-program eller skapa ett nytt.

4. Om du skapar ett nytt Azure AD-program inkluderar du följande information:  

   - **Svars-URL**: URL: en där användarna kan logga in för att använda ditt Azure AD-program.

   - **App-ID-URI**: ett logiskt ID för Azure AD-programmet som presenteras när den skickar en begäran om enkel inloggning till Azure AD.

   - **Säkerhets roller**: roll **hanteraren** (samma som ägar rollen i cpp) och **utvecklaren** (samma som rollen deltagare i cpp) gäller för programmet för kommersiella marknads platser i Partner Center, och de kan ASSOCIERAs med det här Azure AD-programmet.  

## <a name="next-steps"></a>Nästa steg

- [Översikt över den kommersiella marknads platsen i Partner Center](csp-commercial-marketplace-overview.md)