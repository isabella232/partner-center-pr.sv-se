---
title: Azure AD-tjänstens huvudnamn
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du lägger till ett huvudnamn för tjänsten i din Azure AD-klientorganisation. Det innebär att du lägger till ett Azure AD-program (tjänstens huvudnamn) i Partnercenter.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d12bb66574e6bcee60b2a1df1673dc9171fbee2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854935"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Lägga till ett Azure AD-program (tjänstens huvudnamn) i Partnercenter

**Lämpliga roller:** Global administratör

I Commercial Marketplace-programmet i Partnercenter kan du nu lägga till ett Azure AD-program (tjänstens huvudnamn) som en användare i ditt Partnercenter-konto. (Du kunde göra det tidigare i ditt Cloud Partner Portal CPP-konto. Nu när du har migrerat till Partnercenter är CPP-kontot skrivskyddat.)
 
>[!Note] 
>Tjänstens huvudnamn är synonymt med Azure AD-programmet.

## <a name="add-an-azure-ad-application-service-principal"></a>Lägga till ett Azure AD-program (tjänstens huvudnamn)

1. På instrumentpanelen i Partnercenter väljer **du Inställningar** och sedan Inställningar **för utvecklare.**

2. Välj **Användare** och sedan Lägg **till Azure AD-program.**

3. Välj ett befintligt Azure AD-program eller skapa ett nytt.

4. Om du skapar ett nytt Azure AD-program ska du inkludera följande information:  

   - **Svars-URL:** Den URL där användare kan logga in för att använda ditt Azure AD-program.

   - **App-ID-URI:** En logisk identifierare för Azure AD-programmet som visas när den skickar en begäran om enkel inloggning till Azure AD.

   - **Säkerhetsroller:** Rollhanteraren **(samma** som rollen Ägare i CPP) och **Utvecklare** (samma som rollen Deltagare i CPP) gäller för Commercial Marketplace-programmet i Partnercenter och kan associeras med det här Azure AD-programmet.  

## <a name="next-steps"></a>Nästa steg

- [Översikt över den kommersiella marknadsplatsen i Partnercenter](csp-commercial-marketplace-overview.md)