---
title: Azure Cost Management av Cloudyn för kryptografiproviders
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du registrerar Cloudyn-webbappen och använder en hemlig nyckel för den i Partner Center så att du kan använda appen för att spåra användning och kostnader för Azure.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/17/2020
ms.locfileid: "92530996"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>Spåra kund Azure-användning och-kostnader med Azure Cost Management-appen för CSP-partner  

**Gäller för**

- Partnercenter
- Cloud Solution Provider program partners

**Lämpliga roller**

- Global administratör
- Administratörs agent

[Få mer information om Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Innan du börjar
Innan du kan använda Azure Cost Management kontrollerar du att du uppfyller följande krav:

- Du är en partner i Cloud Solution Provider-programmet.
- Du kan skapa en API-webbapp för partner Center.

## <a name="overview"></a>Översikt

Cloudyn är en webbapp som gör att du kan spåra och hantera hur mycket dina kunder använder Azure och kostnaden för den användningen. Du använder det via partner Center API.

## <a name="register-your-web-app-in-the-partner-center"></a>Registrera din webbapp i Partner Center
När du registrerar en Azure Active Directory webbapp i Partner Center ger du åtkomst till Partner Center-API: et. 
1.  Logga in [på Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) med ett [globalt administratörs-eller administratörs agent konto](create-user-accounts-and-set-permissions.md).
2.  Från **partner Center** väljer du **konto inställningar** &gt; **[hantering av appar](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .
3.  I avsnittet **webbapp** klickar du på **Lägg till ny webbapp** .
<br> **Obs** : om du tidigare har skapat en webbapp kan du hoppa över steg 3.
4.  Kopiera och spara **handels-ID-** GUID och GUID för **app-ID** för din webbapp. Du behöver båda ID: na för att använda den 30 dagars kostnads fria utvärderings versionen av Azure Cost Management-appen.

## <a name="add-a-secret-key-to-your-app"></a>Lägg till en hemlig nyckel i appen
1. I list rutan bredvid knappen **Lägg till nyckel** väljer du varaktigheten 1 eller 2 år.
2. Klicka på **Lägg till nyckel** . 
3. Kopiera och spara värdet för den hemliga nyckeln. Du behöver detta för den 30-dagars kostnads fria utvärderings versionen.<br>
   > [!NOTE]  
   > Programmets hemliga nycklar liknar lösen ord med längre förfallo datum. Spara nyckelvärdet på en säker plats för framtida användning.

## <a name="next-steps"></a>Nästa steg
Starta en [30-dagars kostnads fri utvärderings version](https://go.microsoft.com/fwlink/?linkid=857895).
Du behöver följande information för att starta utvärderings versionen:
- Inloggnings uppgifter för partner Center
- GUID för handels-ID
- GUID för app-ID
- Nyckel värde för program hemligt
