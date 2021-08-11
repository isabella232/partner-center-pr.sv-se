---
title: Översikt – CSP Marketplace
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig hur du säljer kundprenumerationer till SaaS-erbjudanden (Programvara som en tjänst) från oberoende programvaruleverantörer (ISV) på marknadsplatsen.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 047738186f93e143e701794b76f8f8f1979129f94129b6fdc79c4de1196f2625
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115690893"
---
# <a name="overview-of-the-commercial-marketplace-in-partner-center"></a>Översikt över den kommersiella marknadsplatsen i Partnercenter

**Lämpliga roller:** Global administratör

Eftersom du är en partner i Molnlösningsleverantör-programmet (CSP) kan du paketa och sälja Microsoft-produkter tillsammans med lösningar som publicerats av oberoende programvaruleverantörer (ISV: er) från tredje part. Genom att kunna paketa lösningar på det här sättet kan du bättre betjäna slutanvändarna och utveckla verksamheten för CSP-tjänster.

Som partner i CSP-programmet kan du använda Partnercenter för att köpa många ISV-lösningar från Microsofts kommersiella marknadsplats. Detta ger dig och dina kunder flera viktiga fördelar:

- Åtkomst till en katalog med programvarulösningar som är optimerade för Microsofts tekniker och miljöer.
- Förenklad kontraktering och förkortad inköpscykel.
- En enda integrering med Partner Center-API:er. (Sådan integrering ger ytterligare åtkomst till en katalog med ISV-lösningar, sänker kostnaden för drift och teknik och effektiviserar hanteringen av flera leverantörsprenumerationer och fakturering via en enda leverantör.)
- Effektiviserad distribution och etablering i kundens Azure-klientorganisation (för vm-baserade lösningar).
- Minskar potentiella utmaningar med direkt ISV-köp eller avtal, konfiguration och integrering av Microsoft-lösningar och behovet av att hantera eller konsolidera återkommande fakturor från flera leverantörer.

## <a name="overview-of-csp-offers-in-the-commercial-marketplace"></a>Översikt över CSP-erbjudanden på den kommersiella marknadsplatsen

Om du är en partner i CSP-programmet finns det många aktiviteter på den kommersiella marknadsplatsen som du kanske vill utföra när det gäller ISV-erbjudanden. I följande tabell kan du läsa mer om varje aktivitet.

|**Om du vill**  |**Läs**   |
|:------------------------------------|:------------------|
|Lär dig hur du visar eller söker efter tillgängliga erbjudanden, priser, produktinformation eller utgivarens kontaktinformation | [Upptäck erbjudanden](csp-commercial-marketplace-discover.md) | 
|Lär dig hur du köper och distribuerar ett erbjudande   | [Inköpserbjudanden](csp-commercial-marketplace-purchase.md)   | 
|Lär dig hur du avbryter eller förnyar en prenumeration eller lägger till eller tar bort licenser  | [Hantera erbjudanden](csp-commercial-marketplace-manage.md) |
|Lär dig mer om hur fakturering fungerar för köp på den kommersiella marknadsplatsen | [Förstå fakturering](csp-commercial-marketplace-billing.md) |
|Lär dig mer om vem som ansvarar för vilka typer av support för ISV-inköp | [Förstå support](csp-commercial-marketplace-support.md) |
|Lär dig mer om kontrakt och ansvarsområden för CSP-partner och ISV:er på den kommersiella marknadsplatsen | [Förstå kontrakt](csp-commercial-marketplace-contracting.md) |

> [!NOTE]
> Den här översikten beskriver hur partner i CSP-programmet kan använda vissa funktioner på den kommersiella marknadsplatsen i Partnercenter. Till skillnad från partner i CSP-programmet har ISV-utgivare en annan marketplace-roll. De har också olika funktioner på Den kommersiella marknadsplatsen som är tillgängliga i Partnercenter. Mer information om isv-utgivares roll finns i Översikt över [Azure Commercial Marketplace.](/azure/marketplace/partner-center-portal/commercial-marketplace-overview)

## <a name="where-to-complete-commercial-marketplace-activities"></a>Var du kan slutföra aktiviteter på den kommersiella marknadsplatsen

Som partner i CSP-programmet kan du slutföra många aktiviteter på den kommersiella marknadsplatsen [](https://partner.microsoft.com/dashboard) för ISV SaaS-erbjudanden direkt från antingen Partner Center-instrumentpanelen eller via [Partner Center-API:er.](/partner-center/develop/) Om du vill slutföra andra Marketplace-aktiviteter kan du dock behöva gå till:

- Den [Microsoft Azure hanteringsportalen](https://portal.azure.com/)

    Eller

- En tredjeparts ISV-utgivares system eller webbplats

Mycket av vart du går för att slutföra aktiviteter börjar med den typ av erbjudande du väljer. Partner i CSP-programmet kan för närvarande göra transaktioner mellan två typer av erbjudanden med ISV-utgivare från tredje part:

1. Licensbaserade SaaS-erbjudanden  
2. Användningsbaserade erbjudanden (inklusive erbjudanden baserade på virtuella datorer, containrar eller Azure-program)

Gå till [Fakturerings grunder om](billing-basics.md) du vill veta mer om hur faktureringen skiljer sig mellan licensbaserade erbjudanden och användningsbaserade erbjudanden.  

Information om var du slutför en specifik Marketplace-aktivitet för licensbaserade eller användningsbaserade ISV-erbjudanden finns i följande tabeller.

|**För licensbaserade eller uppmätta SaaS-erbjudanden från ISV:er**  |**Användning**  |
|:------------------------------------|:------------------|
|Identifiera eller söka efter tillgängliga erbjudanden  | PartnerCenter-instrumentpanelen eller Partnercenter-API:er  |
|Så här köper du ett erbjudande  | PartnerCenter-instrumentpanelen eller Partnercenter-API:er  |
|Distribuera ett köpt erbjudande (kontokonfiguration, programvaruhantering eller distribution i kundens AAD-klient)  | ISV-utgivarens system eller webbplats  |
|Avbryta/förnya erbjudandeprenumerationer eller lägga till/ta bort licenser | PartnerCenter-instrumentpanelen eller Partnercenter-API:er  |
|Skapa användare eller hantera behörigheter  | ISV-utgivarens system eller webbplats  |

|**För användningsbaserade erbjudanden från ISV:er**  |**Användning**  |
|:------------------------------------|:------------------|
|Identifiera eller söka efter tillgängliga erbjudanden  | PartnerCenter-instrumentpanel, Partnercenter-API:er eller Azure Portal  |
|Så här köper du ett erbjudande  | Azure Portal  |
|Distribuera ett köpt erbjudande (kontokonfiguration, programvaruhantering eller distribution i kundens AAD-klient)  | Azure Portal  |
|Avbryta/förnya erbjudandeprenumerationer eller lägga till/ta bort licenser | Azure Portal  |
|Skapa användare eller hantera behörigheter  | Azure Portal  |

## <a name="next-steps"></a>Nästa steg

- [Identifiera eller visa erbjudanden på den kommersiella marknadsplatsen](csp-commercial-marketplace-discover.md)
- [Köpa erbjudanden på den kommersiella marknadsplatsen](csp-commercial-marketplace-purchase.md)
