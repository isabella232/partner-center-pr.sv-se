---
title: Installera Partner Center Analytics för Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Följ stegen i den här artikeln för att installera och förhandsgranska appen Partnercenteranalys för Power BI (för direkta partner i CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a07742a55df088842f6bac1a1cbdd65bf0db8282
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961353"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Installera och förhandsgranska partnercenteranalysappen för Microsoft Power BI


**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Försäljningsagentens | Administratörsagent

## <a name="before-you-begin"></a>Innan du börjar

Välj det program som är mest relevant för din verksamhet från följande lista över tillgängliga Microsoft Power BI appar:

- [Direktprovider](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Indirekt leverantör](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Indirekt återförsäljare](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Innan du installerar förhandsversionen av Partner Center Analytics-appen måste du uppfylla följande krav.

- Du väljer rätt Power BI för din verksamhet.

- Du har en Power BI Pro-licens.

- Du har behörighet att installera mallappar i din klientorganisation.

- Du kan logga in på Power BI.

- Du kan logga in som global administratör, administratörsagent eller faktureringsadministratör för företagets [Azure Active Directory (Azure AD).](azure-active-directory-tenants-and-partner-center.md)

## <a name="to-install-the-app"></a>Så här installerar du appen

1. Välj den länk för appkälla som du fått (Direct Provider/Indirect Provider/Indirect Reseller) i avsnittet ovan.

2. Välj **HÄMTA NU.** 

3. Godkänn villkoren genom att välja **Fortsätt.**

4. Under Har du redan ett konto? välj **Logga in.**

5. På nästa sida anger du ditt Power BI användarnamn och lösenord och väljer sedan **Logga in.**

6. Installera arbetsytan genom att ange arbetsytans namn.

7. Du hittar mallapparna som installerats under Avsnittet Appar.

8. Välj **Appar** och välj de installerade apparna.

9. Kom igång med den nya appskärmen öppnas.

10. Om du vill ansluta till data väljer **du Anslut**.

11. På Anslut till **popup-fönstret Partner Center Analytics** kontrollerar  du att autentiseringsmetoden är inställd på **oAuth2** eller väljer **oAuth2** i listan om den inte är det. 

> [!NOTE]  
>  Det kan ta några minuter innan fönstret visas.

12. På sidan **Partner Center Analytics Connector** loggar du in med autentiseringsuppgifterna för global administratör, administratörsagent eller faktureringsadministratör för ditt företags Azure AD-klientorganisation och väljer sedan Logga **in.**
 
13. När du uppmanas att komma åt väljer du **Acceptera**. 

När Partner Center Analytics-tjänsten är ansluten till Power BI börjar data läsas in. Beroende på mängden data kan det ta upp till 10 minuter. 

När data har läses in kan du börja använda instrumentpanelen och rapporterna i Partnercenter Analytics-appen i Power BI.

## <a name="next-steps"></a>Nästa steg

[Visa dina affärsdata med Partner Center Analytics-appen för Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
