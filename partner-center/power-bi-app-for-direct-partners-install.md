---
title: Installera Partner Center Analytics för Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Följ stegen i den här artikeln för att installera och förhandsgranska appen Partnercenteranalys för Power BI (för direkta partner i CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ff95f989ac847bd2c17558d062c86a52110b2ddf
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565056"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Installera och förhandsgranska partnercenteranalysappen för Microsoft Power BI


**Lämpliga roller:** Globala | Administratörsbehörighet för | Försäljningsagent | Administratörsagent

## <a name="before-you-begin"></a>Innan du börjar

Välj det program som är mest relevant för ditt företag från följande lista över tillgängliga Microsoft Power BI appar:

- [Direkt provider](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Indirekt leverantör](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Indirekt återförsäljare](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Innan du installerar förhandsversionen av Partner Center Analytics-appen måste du se till att du uppfyller följande krav.

- Du väljer rätt Power BI för ditt företag.

- Du har en Power BI Pro-licens.

- Du har behörighet att installera mallappar i din klientorganisation.

- Du kan logga in på Power BI.

- Du kan logga in som global administratör, administratörsagent eller faktureringsadministratör på företagets [Azure Active Directory (Azure AD).](azure-active-directory-tenants-and-partner-center.md)

## <a name="to-install-the-app"></a>Så här installerar du appen

1. Välj länken för appkällan (Direct Provider/Indirect Provider/Indirect Reseller) i avsnittet ovan.

2. Välj **HÄMTA NU.** 

3. Godkänn villkoren genom att välja **Fortsätt.**

4. Under Har du redan ett konto? välj **Logga in.**

5. På nästa sida anger du Power BI användarnamn och lösenord och väljer sedan **Logga in.**

6. Installera arbetsytan genom att ange arbetsytans namn.

7. Du hittar mallapparna som installerats under Avsnittet Appar.

8. Välj **Appar** och välj de installerade apparna.

9. Skärmen Kom igång med din nya app öppnas.

10. Om du vill ansluta till data väljer du **Anslut.**

11. I **popup-fönstret** Anslut till Partner Center Analytics  kontrollerar du att autentiseringsmetoden är inställd på **oAuth2** eller väljer **oAuth2** i listan om den inte är det. 

> [!NOTE]  
>  Det kan ta några minuter innan fönstret visas.

12. På sidan **partnercenteranalysanslutningsapp** loggar du in med autentiseringsuppgifter för global administratör, administratörsagent eller faktureringsadministratör för ditt företags Azure AD-klientorganisation och väljer **sedan Logga in.**
 
13. När du uppmanas att komma åt väljer du **Acceptera.** 

När Partner Center Analytics-tjänsten är ansluten till Power BI börjar data läsas in. Beroende på mängden data kan det ta upp till 10 minuter. 

När data har läses in kan du börja använda instrumentpanelen och rapporterna för Partnercenter Analytics-appen i Power BI.

## <a name="next-steps"></a>Nästa steg

[Visa dina affärsdata med PartnerCenter Analytics-appen för Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
