---
title: Installera Partner Center Analytics för Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Följ stegen i den här artikeln för att installera och förhandsgranska Partner Center Analytics-appen för Power BI (för direkta partner i CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 754b3310918df9b38129cf1374ae3731d9d8062e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215857"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Installera och förhandsgranska partnercenteranalysappen för Microsoft Power BI


**Lämpliga roller**
-   Global administratör
-   Användaradministratör
-   Försäljnings agent
-   Administratörs agent

## <a name="before-you-begin"></a>Innan du börjar

Välj det program som är mest relevant för ditt företag i följande lista med tillgängliga Power BI appar:
- [Direkt Provider](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Indirekt Provider](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Indirekt åter försäljare](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Innan du installerar för hands versionen av Partner Center Analytics-appen kontrollerar du att du uppfyller följande krav.

- Du väljer rätt Power BI app för din verksamhet.

- Du har en licens för Power BI Pro.

- Du har behörighet att installera mallar för appar på din klient organisation.

- Du kan logga in på Power BI.

- Du kan logga in som global administratör, administratörs agent eller fakturerings administratör för [företagets Azure Active Directory (Azure AD)-klient](azure-active-directory-tenants-and-partner-center.md).

## <a name="to-install-the-app"></a>Så här installerar du appen

1. Klicka på länken för den app-källa som angetts (direkt Provider/indirekt Provider/indirekt åter försäljare) i avsnittet ovan.

2. Klicka på **Hämta nu**. 

3. Godkänn de allmänna villkoren genom att klicka på **Fortsätt**.

4. Har du redan ett konto? Välj **Logga** in.

5. Ange ditt Power BI användar namn och lösen ord på nästa sida och välj sedan logga in.

6. Installera arbets ytan genom att ange arbets ytans namn.

7. Du hittar mallens appar som installeras under Apps.

8. Klicka på appar och välj de installerade apparna.

9. Kom igång med din nya app-skärm öppnas.

10. Klicka på **Anslut** för att ansluta till data.

11. I popup-fönstret **Anslut till Partner Center Analytics** kontrollerar du att **autentiseringsmetoden** är inställd på **oAuth2** eller väljer **oAuth2** i listan om den inte är det. 

> [!NOTE]  
>  Det kan ta några minuter innan det här fönstret visas.

12. På sidan **partner Center Analytics Connector** loggar du in med autentiseringsuppgifter för global administratör, administratörs agent eller fakturerings administratör för ditt företags Azure AD-klient och väljer sedan **Logga** in.
 
13. När du tillfrågas om åtkomst väljer du **acceptera**. 

När tjänsten Partner Center Analytics är ansluten till Power BI börjar data läsas in. Beroende på mängden data kan detta ta upp till 10 minuter. 

När data har lästs in kan du börja använda instrument panelen för partner Center Analytics-appen och rapporter i Power BI.

## <a name="next-steps"></a>Nästa steg

[Visa dina affärs data med partner Center Analytics-appen för Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
