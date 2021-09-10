---
title: Azure AD-tjänstens huvudnamn
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Lär dig hur du lägger till ett huvudnamn för tjänsten i din Azure AD-klientorganisation. Det innebär att du lägger till ett Azure AD-program (tjänstens huvudnamn) i Partnercenter.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: a7851d270ad51a5a06ebc7d7725a2ae5c803419b
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961531"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Lägga till ett Azure AD-program (tjänstens huvudnamn) i Partnercenter

**Lämpliga roller:** Global administratör

I Commercial Marketplace-programmet i Partnercenter kan du nu lägga till ett Microsoft Azure Active Directory-program (Azure AD) (tjänstens huvudnamn) som en användare i ditt Partnercenter-konto. (Du kunde göra det tidigare i ditt Cloud Partner Portal-konto (CPP). Nu när du har migrerat till Partnercenter är CPP-kontot skrivskyddat.)
 
>[!Note] 
>Tjänstens huvudnamn är synonymt med Azure AD-programmet.

## <a name="add-an-azure-ad-application-service-principal"></a>Lägga till ett Azure AD-program (tjänstens huvudnamn)

1. På instrumentpanelen i Partnercenter väljer **du Inställningar** och sedan **Utvecklarinställningar.**

2. Välj **Användare** och sedan Lägg **till Azure AD-program.**

3. Välj ett befintligt Azure AD-program eller skapa ett nytt.

4. Om du skapar ett nytt Azure AD-program ska du inkludera följande information:  

   - **Svars-URL:** Den URL där användare kan logga in för att använda ditt Azure AD-program.

   - **App-ID-URI:** En logisk identifierare för Azure AD-programmet som visas när den skickar en begäran om enkel inloggning till Azure AD.

   - **Säkerhetsroller:** Rollhanteraren **(samma** som rollen Ägare i CPP) och **Utvecklare** (samma som rollen Deltagare i CPP) gäller för Commercial Marketplace-programmet i Partnercenter och kan associeras med det här Azure AD-programmet.  

## <a name="next-steps"></a>Nästa steg

- [Översikt över den kommersiella marknadsplatsen i Partnercenter](csp-commercial-marketplace-overview.md)