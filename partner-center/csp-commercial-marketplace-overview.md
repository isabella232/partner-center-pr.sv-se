---
title: Översikt – CSP Marketplace
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Lär dig hur du säljer kundprenumerationer till SaaS-erbjudanden (Programvara som en tjänst) från oberoende programvaruleverantörer (ISV: er) på marknadsplatsen.'
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7c18f69a62e8f8d126a0756911d2fbcdfdb85d8d
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147878"
---
# <a name="overview-of-the-commercial-marketplace-in-partner-center"></a>Översikt över den kommersiella marknadsplatsen i Partnercenter

**Lämpliga roller:** Global administratör

Eftersom du är en partner i Molnlösningsleverantör-programmet (CSP) kan du paketa och sälja Microsoft-produkter tillsammans med lösningar som publicerats av oberoende programvaruleverantörer (ISV) från tredje part. Genom att kunna paketa lösningar på det här sättet kan du bättre betjäna slutkunder och utveckla din CSP-tjänstverksamhet.

Som partner i CSP-programmet kan du använda Partnercenter för att köpa många ISV-lösningar från Microsofts kommersiella marknadsplats. Detta ger dig och dina kunder flera viktiga fördelar:

- Åtkomst till en katalog med programvarulösningar som är optimerade för Microsofts tekniker och miljöer.
- Förenklad kontraktering och förkortad inköpscykel.
- En enda integrering med Partner Center-API:er. (Sådan integrering ger ytterligare åtkomst till en katalog med ISV-lösningar, sänker kostnaden för drift och teknik och effektiviserar hanteringen av flera leverantörsprenumerationer och fakturering via en enda leverantör.)
- Smidig distribution och etablering i kundens Azure-klientorganisation (för virtual machine-baserade lösningar).
- Minskar potentiella utmaningar med direkt ISV-köp eller kontraktering, konfiguration och integrering av Microsoft-lösningar och behovet av att hantera eller konsolidera återkommande fakturor från flera leverantörer.

## <a name="overview-of-csp-offers-in-the-commercial-marketplace"></a>Översikt över CSP-erbjudanden på den kommersiella marknadsplatsen

Om du är en partner i CSP-programmet finns det många aktiviteter på den kommersiella marknadsplatsen som du kanske vill utföra när det gäller ISV-erbjudanden. I följande tabell kan du lära dig mer om varje aktivitet.

|**Om du vill**  |**Läsa**   |
|:------------------------------------|:------------------|
|Lär dig hur du visar eller söker efter tillgängliga erbjudanden, priser, produktinformation eller kontaktinformation för utgivare | [Upptäck erbjudanden](csp-commercial-marketplace-discover.md) | 
|Lär dig hur du köper och distribuerar ett erbjudande   | [Inköpserbjudanden](csp-commercial-marketplace-purchase.md)   | 
|Lär dig hur du avbryter eller förnyar en prenumeration eller lägger till eller tar bort licenser  | [Hantera erbjudanden](csp-commercial-marketplace-manage.md) |
|Lär dig mer om hur fakturering fungerar för köp på den kommersiella marknadsplatsen | [Förstå fakturering](csp-commercial-marketplace-billing.md) |
|Lär dig mer om vem som ansvarar för vilka typer av support för ISV-inköp | [Förstå support](csp-commercial-marketplace-support.md) |
|Lär dig mer om kontrakt och ansvarsområden för CSP-partner och ISV:er på den kommersiella marknadsplatsen | [Förstå kontrakt](csp-commercial-marketplace-contracting.md) |

> [!NOTE]
> Den här översikten beskriver hur partner i CSP-programmet kan använda vissa funktioner på den kommersiella marknadsplatsen i Partnercenter. Till skillnad från partner i CSP-programmet har ISV-utgivare en annan marketplace-roll. De har också olika funktioner på Den kommersiella marknadsplatsen som är tillgängliga i Partnercenter. Mer information om rollen för ISV-utgivare finns i Översikt över [Azure Commercial Marketplace.](/azure/marketplace/partner-center-portal/commercial-marketplace-overview)

## <a name="where-to-complete-commercial-marketplace-activities"></a>Var du kan slutföra aktiviteter på den kommersiella marknadsplatsen

Som partner i CSP-programmet kan du slutföra många aktiviteter på den kommersiella marknadsplatsen [](https://partner.microsoft.com/dashboard) för ISV SaaS-erbjudanden direkt från Partner Center-instrumentpanelen eller via [Partner Center-API:er.](/partner-center/develop/) Om du vill slutföra andra Marketplace-aktiviteter kan du dock behöva gå till:

- Den [Microsoft Azure hanteringsportalen](https://portal.azure.com/)

    Eller

- En tredjeparts ISV-utgivares system eller webbplats

Mycket av vart du går för att slutföra aktiviteter börjar med den typ av erbjudande som du väljer. Partner i CSP-programmet kan för närvarande göra transaktioner med två typer av erbjudanden med isv-utgivare från tredje part:

1. Licensbaserade SaaS-erbjudanden  
2. Användningsbaserade erbjudanden (inklusive erbjudanden baserade på virtuella datorer, containrar eller Azure-program)

Gå till [Grundläggande fakturering om](billing-basics.md) du vill veta mer om hur faktureringen skiljer sig mellan licensbaserade erbjudanden och användningsbaserade erbjudanden.  

Information om var du slutför en specifik Marketplace-aktivitet för licensbaserade eller användningsbaserade ISV-erbjudanden finns i följande tabeller.

|**För licensbaserade eller uppmätta SaaS-erbjudanden från ISV:er**  |**Användning**  |
|:------------------------------------|:------------------|
|Identifiera eller söka efter tillgängliga erbjudanden  | Partner Center-instrumentpanel eller Partner Center-API:er  |
|Så här köper du ett erbjudande  | Partner Center-instrumentpanel eller Partner Center-API:er  |
|Distribuera ett köpt erbjudande (kontokonfiguration, programvaruhantering eller distribution i kundens AAD-klient)  | ISV-utgivarens system eller webbplats  |
|Avbryta/förnya erbjudandeprenumerationer eller lägga till/ta bort licenser | Partner Center-instrumentpanel eller Partner Center-API:er  |
|Skapa användare eller hantera behörigheter  | ISV-utgivarens system eller webbplats  |

|**För användningsbaserade erbjudanden från ISV:er**  |**Användning**  |
|:------------------------------------|:------------------|
|Identifiera eller söka efter tillgängliga erbjudanden  | PartnerCenter-instrumentpanel, PartnerCenter-API:er eller Azure Portal  |
|Så här köper du ett erbjudande  | Azure Portal  |
|Distribuera ett köpt erbjudande (kontokonfiguration, programvaruhantering eller distribution i kundens AAD-klient)  | Azure Portal  |
|Avbryta/förnya erbjudandeprenumerationer eller lägga till/ta bort licenser | Azure Portal  |
|Skapa användare eller hantera behörigheter  | Azure Portal  |

## <a name="next-steps"></a>Nästa steg

- [Identifiera eller visa erbjudanden på den kommersiella marknadsplatsen](csp-commercial-marketplace-discover.md)
- [Köpa erbjudanden på den kommersiella marknadsplatsen](csp-commercial-marketplace-purchase.md)
