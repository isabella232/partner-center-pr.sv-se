---
title: Påbörja flytten till Azure-planen
description: Lär dig vad du och dina kunder behöver veta om att använda Azures betala enligt plan, inklusive första steg, säkerhetsåtgärder och hur du kommer igång.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 58feabdefb02660559c69f61190070310768b947
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149663"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Börja använda Betala enligt användning-priser med Azure-planen

**Lämpliga roller:** Administratörsagent | Försäljningsagent


Microsoft har introducerat en ny handelsupplevelse i Partnercenter.  Med den här nya handelsupplevelsen får partner tillgång till Azure-tjänster till betala-enligt användning-priser för kunder under Microsoft-kundavtal.

Den här planen förenklar köpupplevelsen – du kan ha flera Azure-prenumerationer i en Azure-plan. Du behöver inte längre skicka en separat order per Azure-prenumeration. Och i den här nya handelsupplevelsen för Azure har vi anpassat oss till en enda global prisprincip som gör det möjligt för CSP-partner att erbjuda Azure till de publicerade priserna.

Våra kunders behov av digital omvandling kräver nya kunskaper från partner. Många kunder letar efter partner som tillhandahåller tjänster utöver transaktionen för att göra molnresan smidigare och hjälpa till att använda Azure-tjänster effektivt. Microsoft-partner spelar en viktig roll i alla steg i kundens livscykel. Dessa typer av partnertjänster är på gång och omfattar övervakning av Azure-egendom, princip- och styrningshantering, konfigurationsjustering, teknisk support och en mängd andra tjänster. De kräver att en partner är bekant med kundens Azure-miljö och har kontinuerlig och lämplig styrning och kontroll över de underliggande resurser som de hanterar. Faktureringspartner som tillhandahåller den här molndriftshanteringen dygnet runt blir berättigade till partner-intjänad kredit för tjänster som **hanteras** för arbetet.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Kontrollera att dina kunder har signerat Microsoft-kundavtal

Sedan den 1 oktober 2019 finns Microsoft-kundavtal ett permanent avtal som förenklar och effektiviserar kundernas köpupplevelse med en helt digital process. Alla kunder som vill dra nytta av den nya handelsupplevelsen i CSP för Azure måste signera Microsoft-kundavtal.

Partner som vill göra en åtgärd enligt den nya Azure-planen och göra en ny beställning bör bekräfta kundens godkännande av Microsoft-kundavtal via instrumentpanelen i Partnercenter och API:et i produktion.

Från och med 1 februari 2020 tas Microsoft Cloud-avtal bort från CSP-programmet. Från och med då krävs en partnerbekräftelse (attestation) av kundens godkännande för den nya Microsoft-kundavtal för alla andra erbjudanden, inklusive Microsoft 365, Dynamics 365 och befintligt Azure. Partner i CSP:en kommer inte att kunna göra en ny beställning för kunden utan att Microsoft-kundavtal.

Fullständig information finns i [Bekräfta kundens godkännande av Microsoft-kundavtal](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>Metoder för säkerhet och åtkomstkontroll

För att hjälpa till att skydda partner och kunder introducerar vi en uppsättning obligatoriska säkerhetskrav för rådgivare, Kontrollpanelen-leverantörer och partner som deltar i Molnlösningsleverantör program.

Partner som inte implementerar de obligatoriska säkerhetskraven kommer inte att kunna genomföra transaktioner i Molnlösningsleverantör-programmet eller hantera kundklienter som utnyttjar delegerade administratörsrättigheter när dessa krav har verkställts. Vi håller på att upprätta ett tekniskt framtvingandedatum för kraven och kommer att meddela partner om datumet med detaljerad information.

## <a name="actions-to-take-to-implement-mfa"></a>Åtgärder att vidta för att implementera MFA

Eftersom vi är en partner med hög behörighet måste vi se till att varje användare har en MFA-utmaning för varje enskild autentisering. Detta kan åstadkommas på något av följande sätt:

- Implementera Azure AD Premium och se till att multifaktorautentisering (MFA) tillämpas för varje användare
- Implementera [standardinställningarna för Azure AD-säkerhet](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementera en lösning från tredje part och se till att MFA tillämpas för varje användare

Från och med 1 augusti 2019 måste alla partner framtvinga multifaktorautentisering för alla användare, inklusive tjänstkonton, i sin partnerklientorganisation. Detaljerad information om dessa säkerhetskrav finns i Säkerhetskrav [för partner.](partner-security-requirements.md)

Microsoft rekommenderar partner att noggrant använda RBAC enligt bästa praxis som aktiveras via Azure Active Directory Privileged Identity Management [resurser.](/azure/active-directory/privileged-identity-management/pim-configure)

## <a name="read-more-about-the-azure-plan"></a>Läs mer om Azure-planen

- [Köpa en Azure-plan](purchase-azure-plan.md)

- [Jämföra Azure-erbjudanden](compare-azure-offers.md)

- [Partner-intjänad kredit – översikt](partner-earned-credit.md)

- Beräkningarna av partners intjänade kredit (PEC) och de roller och behörigheter som är berättigade att tjäna partnertjänade krediter är tillgängliga från prislistan för instrumentpanelen i Partnercenter (inloggning krävs).

## <a name="next-steps"></a>Nästa steg 

- [Så bestäms partnerns intjänade kredit – information](partner-earned-credit-explanation.md)
- [Förklaring av prislista för Azure-plan](azure-plan-price-list.md)
- [Överföra dina kunder till Azure-planen](azure-plan-transition.md)
- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
- [En fullständig lista över länder/regioner där Azure-planen är tillgänglig](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)