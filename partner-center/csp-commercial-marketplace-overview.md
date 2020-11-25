---
title: Översikt – KRYPTOGRAFIPROVIDER Marketplace
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du säljer kund prenumerationer till SaaS-erbjudanden från oberoende program varu leverantörer (ISV) på Marketplace.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c8d64167261fe9f425a1430ac0c109b446b50913
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038837"
---
# <a name="overview-of-the-commercial-marketplace-in-partner-center"></a>Översikt över den kommersiella marknads platsen i Partner Center

**Gäller för**

- Partnercenter
- Partner i CSP-programmet

Att vara en partner i ett CSP-program (Cloud Solution Provider) gör att du kan paketera och sälja Microsoft-produkter tillsammans med lösningar som publicerats av oberoende program varu leverantörer (ISV: er). Att kunna paketera lösningar på det här sättet gör att du bättre kan betjäna slutanvändare och utveckla din verksamhet för CSP-tjänster.

Som partner i CSP-programmet kan du använda Partner Center för att köpa många ISV-lösningar från Microsofts kommersiella marknads plats. Detta ger dig och dina kunder flera viktiga fördelar:

- Åtkomst till en katalog med program lösningar som är optimerade för Microsofts tekniker och miljöer.
- Förenklad avtals slutande och kortare inköps cykel.
- En enkel integrering med API: er för partner Center. (Sådan integrering ger ytterligare åtkomst till en katalog med ISV-lösningar, sänker kostnaderna för drift och teknik och effektiviserar hanteringen av flera leverantörs prenumerationer och fakturering genom en enda leverantör.)
- Effektiviserad distribution och etablering i kundens Azure-klient (för virtuella datorbaserade lösningar).
- Minskar potentiella utmaningar med direkt ISV-köp eller avtals slutande, Microsofts lösnings konfiguration och integrering och behovet av att hantera eller konsolidera återkommande fakturor från flera leverantörer.

## <a name="overview-of-csp-offers-in-the-commercial-marketplace"></a>Översikt över CSP-erbjudanden på den kommersiella marknaden

Om du är en partner i CSP-programmet finns det många kommersiella Marketplace-aktiviteter som du kanske vill utföra i avseende på ISV-erbjudanden. I följande tabell finns mer information om varje aktivitet.

|**Om du vill**  |**Läs**   |
|:------------------------------------|:------------------|
|Lär dig att visa eller söka efter tillgängliga erbjudanden, priser, produkt information eller information om utgivarens kontakt information | [Identifiera erbjudanden](csp-commercial-marketplace-discover.md) | 
|Lär dig hur du köper och distribuerar ett erbjudande   | [Inköps erbjudanden](csp-commercial-marketplace-purchase.md)   | 
|Lär dig hur du avbryter eller förnyar en prenumeration eller lägger till eller tar bort licenser  | [Hantera erbjudanden](csp-commercial-marketplace-manage.md) |
|Lär dig mer om hur faktureringen fungerar för inköp av kommersiella marknads platser | [Förstå fakturering](csp-commercial-marketplace-billing.md) |
|Läs om vem som är ansvarig för vilka typer av stöd för ISV-köp | [Förstå support](csp-commercial-marketplace-support.md) |
|Läs om avtal och ansvars områden för CSP-partner och ISV: er på den kommersiella marknaden | [Förstå avtals slutande](csp-commercial-marketplace-contracting.md) |

> [!NOTE]
> Den här översikten beskriver hur partner i CSP-programmet kan använda vissa kommersiella Marketplace-funktioner i Partner Center. Till skillnad från partner i CSP-programmet har ISV-utgivare en annan Marketplace-roll. De har också olika kommersiella Marketplace-funktioner som är tillgängliga för dem i Partner Center. Mer information om ISV-utgivarens roll finns i [Översikt över Azures kommersiella marknads platser](/azure/marketplace/partner-center-portal/commercial-marketplace-overview).

## <a name="where-to-complete-commercial-marketplace-activities"></a>Så här slutför du aktiviteter på den kommersiella marknaden

Som partner i CSP-programmet kan du utföra många kommersiella Marketplace-aktiviteter för ISV SaaS-erbjudanden direkt från antingen Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard) eller med hjälp av [API: er för partner Center](/partner-center/develop/). För att slutföra andra Marketplace-aktiviteter kan du dock behöva gå till:

- [Microsoft Azure hanterings Portal](https://portal.azure.com/)

    Eller

- En tredjeparts ISV-utgivares system eller webbplats

Mycket av vart du går för att slutföra aktiviteter börjar med den typ av erbjudande du väljer. Partner i CSP-programmet kan för närvarande använda två typer av erbjudanden med ISV-utgivare från tredje part:

1. Licensbaserade SaaS-erbjudanden  
2. Användnings erbjudanden (inklusive erbjudanden baserade på virtuella datorer, behållare eller Azure-program)

Gå till [grunderna för fakturering](billing-basics.md) för att lära dig mer om hur faktureringen skiljer sig mellan licensbaserade erbjudanden och användnings erbjudanden.  

Se följande tabeller för att lära dig var du ska slutföra en speciell Marketplace-aktivitet för licensbaserade eller användnings ISV-erbjudanden.

|**För licensbaserade eller avgiftsbelagda SaaS-erbjudanden från ISV: er**  |**Användning**  |
|:------------------------------------|:------------------|
|Identifiera eller Sök efter tillgängliga erbjudanden  | API: er för partner Center eller partner Center  |
|Köpa ett erbjudande  | API: er för partner Center eller partner Center  |
|Så här distribuerar du ett inköpt erbjudande (konto inställningar, program varu hantering eller distribution i kundens AAD-klient)  | ISV-utgivarens system eller webbplats  |
|Så här avbryter/förnyar du erbjudande prenumerationer eller Lägg till/ta bort licenser | API: er för partner Center eller partner Center  |
|Skapa användare eller hantera behörigheter  | ISV-utgivarens system eller webbplats  |

|**För användnings erbjudanden från ISV: er**  |**Användning**  |
|:------------------------------------|:------------------|
|Identifiera eller Sök efter tillgängliga erbjudanden  | Instrument panel för partner Center, API: er för partner Center eller Azure Portal  |
|Köpa ett erbjudande  | Azure Portal  |
|Så här distribuerar du ett inköpt erbjudande (konto inställningar, program varu hantering eller distribution i kundens AAD-klient)  | Azure Portal  |
|Så här avbryter/förnyar du erbjudande prenumerationer eller Lägg till/ta bort licenser | Azure Portal  |
|Skapa användare eller hantera behörigheter  | Azure Portal  |

## <a name="next-steps"></a>Nästa steg

- [Identifiera eller Visa erbjudanden på kommersiella Marketplace](csp-commercial-marketplace-discover.md)
- [Köp kommersiella Marketplace-erbjudanden](csp-commercial-marketplace-purchase.md)