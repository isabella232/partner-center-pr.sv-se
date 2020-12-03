---
title: Påbörja flytten till Azure-planen
description: Lär dig mer om vad du och dina kunder behöver veta om hur du använder Azures betala per användning-plan, inklusive första stegen, säkerhets åtgärder och hur du kommer igång.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: fcf75acef4afb80c5aec889911ffc2b4a53b6edd
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534921"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Börja använda betala per användning-pris med Azure-prenumerationen

**Lämpliga roller**

- Administratörs agent
- Försäljnings agent


Microsoft har lanserat en ny Commerce-upplevelse i Partner Center.  Med den nya Commerce-upplevelsen får partners till gång till Azure-tjänster med betala per användning-pris för kunder enligt Microsofts kund avtal.

Den här planen fören klar köp upplevelsen – du kan ha flera Azure-prenumerationer i en Azure-plan. Du behöver inte längre skicka en separat order per Azure-prenumeration. I den här nya Commerce Experience för Azure har vi justerat till en enda global pris princip som gör det möjligt för CSP-partner att erbjuda Azure till de publicerade priserna.

Våra kunders digitala omvandlings behov kräver nya kunskaper från partner. Många kunder letar efter partner för att tillhandahålla tjänster ovan och bortom transaktionen för att göra sin moln resa smidigare och hjälpa att använda Azure-tjänster på ett effektivt sätt. Microsoft-partner spelar en viktig roll i alla stadier av kund livs cykeln. De här typerna av partner tjänster är av olika slag och innefattar hantering av Azure-egendom, princip-och styrnings hantering, installation och konfiguration fin justering, teknisk support och flera olika tjänster. De kräver att en partner är väl bekant med kundens Azure-miljö och har kontinuerlig och lämplig styrning och kontroll över de underliggande resurser som de hanterar. Fakturerings partner som tillhandahåller den här 24 X 7-moln drifts hanteringen blir berättigade till en **partner med intjänad kredit för tjänster som hanteras** för det arbetet.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Se till att dina kunder har undertecknat Microsofts kund avtal

Sedan den 1 oktober 2019 är Microsofts kund avtal ett avtal som gör det möjligt att förenkla och effektivisera kund inköps upplevelsen med en helt digital process. Alla kunder som vill dra nytta av den nya Commerce-upplevelsen i CSP för Azure måste teckna Microsofts kund avtal.

Partner som vill använda Transact under den nya Azure-planen och göra en ny beställning bör bekräfta kund godkännande av Microsofts kund avtal med hjälp av instrument panelen för partner Center och API i produktion.

Med början den 1 februari 2020 tas det befintliga Microsoft Clouds avtalet bort från CSP-programmet. Från och med den tiden krävs partner bekräftelse (attestering) av kundens godkännande för det nya Microsofts kund avtal för alla andra erbjudanden, inklusive Microsoft 365, Dynamics 365 och befintliga Azure. Partner i CSP kommer inte att kunna skapa en ny order för kunden utan attestering av Microsofts kund avtal.

För fullständig information, Läs [bekräfta kund godkännande av Microsofts kund avtal](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>Säkerhets-och åtkomst kontroll metoder

För att hjälpa till att skydda partner och kunder, introducerar vi en uppsättning obligatoriska säkerhets krav för rådgivare, kontroll panels leverantörer och partner som ingår i Cloud Solution Provider-programmet.

Partner som inte implementerar de obligatoriska säkerhets kraven kommer inte att kunna använda Transact i Cloud Solution Provider-programmet eller hantera kund klienter som utnyttjar ombuds administratörs rättigheter när dessa krav tillämpas. Vi håller på att upprätta ett tekniskt tvångs datum för kraven och kommer att meddela partners om datumet med detaljerad information.

## <a name="actions-to-take-to-implement-mfa"></a>Åtgärder som ska vidtas för att implementera MFA

Med hänsyn till att varje användare har en MFA-utmaning för varje enskild autentisering, är det viktigt att du har en partner som har hög privilegier. Detta kan åstadkommas på något av följande sätt:

- Implementera Azure AD Premium och se till att Multi-Factor Authentication (MFA) tillämpas för varje användare
- Implementera [standardinställningar för Azure AD-säkerhet](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementera en lösning från tredje part och se till att MFA upprätthålls för varje användare

Från och med 1 augusti 2019 krävs alla partner för att genomdriva Multi-Factor Authentication för alla användare, inklusive tjänst konton, i sin partner klient. Detaljerad information om de här säkerhets kraven finns på [partner säkerhets krav](partner-security-requirements.md).

Microsoft rekommenderar att partners använder RBAC-och följande metod tips som är aktiverade via [Azure Active Directory Privileged Identity Management-resurser](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="read-more-about-the-azure-plan"></a>Läs mer om Azure-prenumerationen

- [Köpa en Azure-plan](purchase-azure-plan.md)

- [Jämföra Azure-erbjudanden](compare-azure-offers.md)

- [Partner intjänad kredit – översikt](partner-earned-credit.md)

- Beräkningarna av partner intjänade kredit (PEC) och de roller och behörigheter som är berättigade till att tjäna partner intjänade krediter är tillgängliga från Partner Center Dashboard pris lista (inloggning krävs).

## <a name="next-steps"></a>Nästa steg 

- [Hur den intjänade krediten för partner fastställs – information](partner-earned-credit-explanation.md)
- [Förklaring av pris lista för Azure-plan](azure-plan-price-list.md)
- [Överföra dina kunder till Azure-planen](azure-plan-transition.md)
- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
- [En fullständig lista över länder/regioner där Azure plan är tillgängligt](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)