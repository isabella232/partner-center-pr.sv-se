---
title: Begär en SLA-kredit från Microsoft
ms.topic: article
ms.date: 03/31/2021
description: Lär dig fördelarna, begränsningarna och procedurerna för att begära en SLA-kredit (serviceavtal) från Microsoft om dina kunder drabbas av ett tjänstavbrott.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 3a0bb85143efe3d4135b56985b9a04e2dbe5e4cc
ms.sourcegitcommit: 57442bbbef15a70bd9a042642140cbf2c8608b09
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/09/2021
ms.locfileid: "113519450"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Hur och när du ska begära en SLA-kredit (serviceavtal) från Microsoft

**Lämpliga roller:** Administratörsagent | Global administratör

Du kan begära **serviceavtalskrediter (SLA)** från Microsoft om en tjänst som du tillhandahåller för dina kunder har ett avbrott.

## <a name="sla-credit-calculation"></a>Beräkning av SLA-kredit

SLA-krediter från Microsoft bestäms baserat på vilka tjänster som har påverkats. Om kunden till exempel har en Office 365-svit men bara upplever ett SharePoint-avbrott godkänns SLA-krediten endast för SharePoint och inte kundens hela plan.

*Krediter är pro-klassificerade baserat på den tjänst som påverkas och varaktigheten för avbrottet.* Information om vilka typer av scenarier som är kvalificerade för SLA-krediter finns i [dokumentet Konsoliderat serviceavtal för Online Services.](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Den här informationen gäller även för tjänster som säljs via Molnlösningsleverantör-programmet (CSP).


## <a name="request-an-sla-credit"></a>Begära en SLA-kredit

*CSP-partnern måste skicka anspråket och all nödvändig information i slutet av kalendermånaden efter den månad då incidenten inträffade.* Om incidenten till exempel inträffade den 15 februari måste Microsoft ta emot anspråket och all nödvändig information senast den 31 mars. Slutanvändare och indirekta återförsäljare kan inte skicka anspråk på SLA-kredit; antingen den indirekta leverantören eller partnern med direktfakturering måste skicka anspråk för sin räkning.

> [!NOTE]
> Rådgivningsincidenter är vanligtvis inte berättigade till SLA-krediter. En incident som skickas till Service Health-instrumentpanelen  anger att en klientorganisation kan påverkas och representerar den bästa information som Microsoft har vid tidpunkten för publiceringen. Hälsosidans data representerar den allmänna tillgängligheten för en tjänst. Påverkan, minskning och lösning av enskilda tjänster kan variera. Mer information finns i den slutliga incidentgranskningen efter och efter incidentgranskningen. Mer [information finns i Kontrollera Microsoft 365 tjänstens](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) hälsa.

### <a name="required-information"></a>Nödvändig information

Kundnamn, klientorganisationsidentifierare, partnerbiljett# och biljett som skapats för datum/tid-stämpel är inte tillräckliga för att ett anspråk ska bearbetas.

Innan du [skickar en SLA-kreditbegäran](#submit-sla-credit-request) till Microsoft måste du samla in **all** följande information som ska ingå i din supportbegäran:

- Kundklientens GUID
- Identifieraren [för avbrottsincidenten](#outage-incident-identifier)?
- Bevis på att kunden har påverkats av avbrottet och har begärt en SLA-kredit.
- Köptes de påverkade prenumerationerna via CSP? *(Ja* eller *nej)*

#### <a name="evidence-that-proves-customer-impact"></a>Bevis som bevisar kundpåverkan

- Information om tid och varaktighet för stilleståndstiden
- Antal och platser för berörda användare (om tillämpligt)
- Beskrivningar av dina försök att lösa incidenten vid tidpunkten för händelsen
- Ett e-postmeddelande från den påverkade kunden som begär support och därefter kredit
- Supportbiljettnumret och information om kundkontakten för att lösa påverkan på tjänsten


#### <a name="outage-incident-identifier"></a>Identifierare för avbrottsincident

Du hittar identifieraren för avbrottsincidenten **på Service Health** i Administrationscenter för Microsoft 365. **Incident-ID för** avbrott är ett tal som föregås av en tvåbokstavsförkortning som anger den berörda tjänsten (till exempel *EX25194* för Exchange Online avbrott). I följande tabell beskrivs vanliga tjänstförkortningar:

| Förkortning med två bokstäver | Microsoft-tjänst |
| ----------------------- | ----------------- |
| Ex | Exchange Online |
| Fo | Exchange Online Protection |
| Sb | Skype för företag Online (tidigare Lync Online) |
| Operativsystem | Office Prenumeration |
| PB | Power BI för Office 365 |
| Sp | sharepoint online |
| Ya | Yammer Enterprise |
| MO | Portalfel |

### <a name="submit-sla-credit-request"></a>Skicka en SLA-kreditbegäran

Så här skickar du din SLA-kreditbegäran till Microsoft via instrumentpanelen i Partnercenter:

1. Logga in på instrumentpanelen i Partnercenter.
2. I den vänstra menyn väljer du **Tjänstförfrågningar och** sedan **Partnersupportbegäranden.**
3. På sidan **Partnerbegäran** väljer du **Ny begäran.**
4. På sidan **Starta begäran hittar** du avsnittet **CSP – kunder, beställningar och prenumerationer**. I det här avsnittet väljer **du Välj en typ av problem** och sedan **Kreditförfrågningar för kundtjänster.**
5. På sidan **Rekommenderade lösningar,** under **Behöver du mer hjälp?** väljer du **Ja.**
6. På sidan **Information** fyller du i **avsnittet Probleminformation.** I **textrutan** Information måste du ange den information som [du samlade](#required-information) in tidigare.
7. Välj **Skicka** för att skicka i din SLA-kreditförfrågan.

## <a name="next-steps"></a>Nästa steg

- [Rapportera problem åt din kund](report-problems-on-behalf-of-a-customer.md)
