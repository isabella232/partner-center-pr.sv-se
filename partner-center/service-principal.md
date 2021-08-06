---
title: Azure AD-tjänstens huvudnamn
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Ta reda på hur du lägger till ett huvudnamn för tjänsten i din Azure AD-klientorganisation. Det innebär att du lägger till ett Azure AD-program (tjänstens huvudnamn) i Partnercenter.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 4b02359403cdf19999ff007de0fa5890f4222163dcb29a0c3070ba7b61ba490e
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115678211"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Lägga till ett Azure AD-program (tjänstens huvudnamn) i Partnercenter

**Lämpliga roller:** Global administratör

I programmet för den kommersiella marknadsplatsen i Partnercenter kan du nu lägga till ett Microsoft Azure Active Directory-program (Azure AD) (tjänstens huvudnamn) som en användare i ditt Partnercenter-konto. (Du kunde göra det tidigare i ditt Cloud Partner Portal-konto (CPP). Nu när du har migrerat till Partnercenter är CPP-kontot skrivskyddat.)
 
>[!Note] 
>Tjänstens huvudnamn är synonymt med Azure AD-programmet.

## <a name="add-an-azure-ad-application-service-principal"></a>Lägga till ett Azure AD-program (tjänstens huvudnamn)

1. Från instrumentpanelen i Partnercenter väljer **du Inställningar** och sedan Inställningar **för utvecklare.**

2. Välj **Användare** och sedan Lägg **till Azure AD-program.**

3. Välj ett befintligt Azure AD-program eller skapa ett nytt.

4. Om du skapar ett nytt Azure AD-program ska du inkludera följande information:  

   - **Svars-URL:** Den URL där användare kan logga in för att använda ditt Azure AD-program.

   - **App-ID-URI:** En logisk identifierare för Azure AD-programmet som visas när den skickar en begäran om enkel inloggning till Azure AD.

   - **Säkerhetsroller:** Rollhanteraren **(samma** som rollen Ägare i CPP) och Utvecklare **(samma** som rollen Deltagare i CPP) gäller för programmet För kommersiell marknadsplats i Partnercenter och kan associeras med det här Azure AD-programmet.  

## <a name="next-steps"></a>Nästa steg

- [Översikt över den kommersiella marknadsplatsen i Partnercenter](csp-commercial-marketplace-overview.md)