---
title: Begär en SLA-kredit från Microsoft
ms.topic: article
ms.date: 04/28/2020
description: Lär dig fördelarna, begränsningarna och procedurerna för att begära ett service avtal (SLA) kredit från Microsoft om kunderna upplever ett tjänst avbrott.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: cb8f6b2280318427b2015403b528fc288ef64d97
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/14/2020
ms.locfileid: "92529222"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Hur och när du ska begära en kredit på service nivå avtal från Microsoft

Du kan begära **service avtals krediter (SLA)** från Microsoft om en tjänst som du tillhandahåller för dina kunder har ett avbrott.

## <a name="sla-credit-calculation"></a>Beräkning av SLA-kredit

SLA-krediter från Microsoft bestäms utifrån vilken eller vilka tjänster som påverkades. Om din kund exempelvis har en Office 365-svit men bara har drabbats av ett SharePoint-avbrott, godkänns SLA-krediten endast för SharePoint och inte kundens hela plan.

*Krediterna klassificeras baserat på den berörda tjänsten och drifts tiden.* Information om vilka typer av scenarier som är kvalificerade för SLA-krediter finns i [Online Services-konsoliderade SLA-dokument](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). Den här informationen gäller endast tjänster som säljs via Cloud Solution Provider-programmet.

## <a name="request-an-sla-credit"></a>Begär en kredit service avtal

*Leverantören av moln lösnings leverantören (CSP) måste skicka in anspråket och all nödvändig information i slutet av kalender månaden efter den månad då incidenten inträffade.* Om incidenten exempelvis skedde 15 februari måste Microsoft ta emot anspråket och all nödvändig information från 31 mars. Slutanvändare och indirekta åter försäljare kan inte skicka anspråk på SLA kredit. antingen måste den indirekta providern eller direkt fakturerings partnern skicka anspråk för deras räkning.

### <a name="required-information"></a>Nödvändig information

Innan du [skickar en kredit förfrågan för SLA](#submit-sla-credit-request) till Microsoft måste du samla in följande information som du kan ta med i support ärendet:

- Kundens klient-GUID
- [Incident identifieraren för avbrott](#outage-incident-identifier)?
- Har de påverkade prenumerationerna köpts via CSP? ( *Ja* eller *Nej* )

#### <a name="outage-incident-identifier"></a>Incident identifierare för avbrott

Du hittar identifieraren för avbrotts incidenten på sidan **service Health** i Microsoft 365 administrations Center. **Incident-ID: t för avbrott** är ett tal som föregås av en förkortning med två bokstäver som indikerar den berörda tjänsten (till exempel *EX25194* för ett Exchange Online-avbrott). I följande tabell beskrivs vanliga tjänst förkortningar:

| Förkortning med två bokstäver | Microsoft-tjänst |
| ----------------------- | ----------------- |
| PRISET | Exchange Online |
| DETALJERADE | Exchange Online-skydd |
| SA | Skype för företag – Online (tidigare Lync Online) |
| Operativsystem | Office-prenumeration |
| PB | Power BI för Office 365 |
| SP | sharepoint online |
| YA | Yammer Enterprise |
| MO | Portal fel |

### <a name="submit-sla-credit-request"></a>Skicka in SLA kredit förfrågan

Skicka din begäran om SLA kredit till Microsoft via instrument panelen för partner Center:

1. Logga in på Partner Center-instrumentpanelen.
2. I den vänstra menyn väljer du **tjänst begär Anden** och väljer sedan **partner support förfrågningar** .
3. På sidan **partner förfrågan** väljer du **ny begäran** .
4. På sidan **Starta begäran** hittar du avsnittet **CSP-kunder, beställningar och prenumerationer** . I det här avsnittet väljer du **Välj en ärende typ** och väljer sedan **kund tjänster kredit förfrågningar** .
5. På sidan **rekommenderade lösningar** under **behöver du mer hjälp?** , Välj **Ja** .
6. Fyll i avsnittet **problem information** på sidan **information** . I text rutan **information** , se till att ange den [information](#required-information) som du tidigare har samlat in.
7. Välj **Skicka** för att skicka i din kredit förfrågan för SLA.
