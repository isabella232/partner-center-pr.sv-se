---
title: Begär en SLA-kredit från Microsoft
ms.topic: article
ms.date: 03/31/2021
description: Lär dig om fördelar, begränsningar och procedurer för att begära en servicenivåavtalskredit (SLA) från Microsoft om dina kunder drabbas av ett tjänstavbrott.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: d98130f22fee81a50b40b8ae08a3fcf909201389
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114839693"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Hur och när du ska begära en SLA-kredit (serviceavtal) från Microsoft

**Lämpliga roller:** Administratörsagent | Global administratör

Du kan begära **serviceavtalskrediter (SLA)** från Microsoft om en tjänst som du tillhandahåller för dina kunder har ett avbrott.

## <a name="sla-credit-calculation"></a>Beräkning av SLA-kredit

SLA-krediter från Microsoft bestäms baserat på vilka tjänster som påverkades. Om kunden till exempel har en Office 365-svit men bara upplever ett SharePoint-avbrott godkänns SLA-krediten endast för SharePoint och inte kundens hela plan.

*Krediterna är klassificerade baserat på den tjänst som påverkas och varaktigheten för avbrottet.* Information om vilka typer av scenarier som är berättigade till SLA-krediter finns i [dokumentet Konsoliderat serviceavtal för Online Services.](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Den här informationen gäller även för tjänster som säljs via Molnlösningsleverantör-programmet (CSP).


## <a name="request-an-sla-credit"></a>Begära en SLA-kredit

*CSP-partnern måste skicka anspråket och all nödvändig information i slutet av kalendermånaden efter den månad då incidenten inträffade.* Om incidenten till exempel inträffade den 15 februari måste Microsoft ta emot anspråket och all nödvändig information senast den 31 mars. Slutanvändare och indirekta återförsäljare kan inte skicka SLA-kreditanspråk; antingen den indirekta leverantören eller partnern med direktfakturering måste skicka anspråk för sin räkning.

> [!NOTE]
> Rådgivningsincidenter är vanligtvis inte berättigade till SLA-krediter. En incident som publiceras på Service Health-instrumentpanelen anger att en klientorganisation kan påverkas och representerar den bästa informationen som Microsoft har vid tidpunkten för publiceringen.  Hälsosidans data representerar en tjänsts allmänna tillgänglighet. Påverkan, minskning och lösning av enskilda tjänster kan variera. Mer information finns i den slutliga incidentgranskningen efter incidenten och efter incidentgranskningen. Mer [information finns i Kontrollera Microsoft 365 tjänsthälsa.](/microsoft-365/enterprise/view-service-health#incidents-and-advisories)

### <a name="required-information"></a>Nödvändig information

Kundnamn, klientorganisations-ID, partnerbiljett# och biljett som skapats för datum/tid-stämpel räcker inte för att ett anspråk ska bearbetas.

Innan du [skickar en begäran om SLA-kredit](#submit-sla-credit-request) till Microsoft måste du samla in **all** följande information som ska ingå i din supportbegäran:

- Kundens klientorganisations GUID
- Identifieraren [för avbrottsincidenten](#outage-incident-identifier)?
- Bevis på att kunden har påverkats av avbrottet och har begärt en SLA-kredit.
- Köptes de påverkade prenumerationerna via CSP? (*Ja* eller *nej*)

#### <a name="evidence-that-proves-customer-impact"></a>Bevis som bevisar kundpåverkan

- Information om tid och varaktighet för stilleståndstiden
- Antal och platser för berörda användare (om tillämpligt)
- Beskrivningar av dina försök att lösa incidenten vid tidpunkten för händelsen
- Ett e-postmeddelande från den påverkade kunden som begär support och därefter kredit
- Supportbiljettens nummer och information om kundkontakten för att lösa påverkan på tjänsten


#### <a name="outage-incident-identifier"></a>Identifierare för avbrottsincident

Du hittar identifieraren för avbrottsincidenten på **Service Health** i Administrationscenter för Microsoft 365. **Id:t för** avbrottsincident är ett tal som föregås av en förkortning med två bokstäver som anger den berörda tjänsten (till exempel *EX25194* för ett Exchange Online avbrott). I följande tabell beskrivs vanliga förkortningar för tjänsten:

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

### <a name="submit-sla-credit-request"></a>Skicka en begäran om SLA-kredit

Så här skickar du din SLA-kreditbegäran till Microsoft via instrumentpanelen i Partnercenter:

1. Logga in på instrumentpanelen i Partnercenter.
2. I den vänstra menyn väljer du **Tjänstförfrågningar och** sedan **Partnersupportbegäranden.**
3. På sidan **Partnerbegäran** väljer du **Ny begäran.**
4. På sidan **Starta begäran hittar** du avsnittet **CSP – kunder, beställningar och prenumerationer**. I det här avsnittet väljer **du Välj en problemtyp** och sedan Customer services credit requests (Kreditförfrågningar **för kundtjänster).**
5. På sidan **Rekommenderade lösningar,** under **Behöver du mer hjälp?** väljer du **Ja.**
6. På sidan **Information** fyller du i **avsnittet Probleminformation.** I **textrutan** Information måste du ange den information som [du](#required-information) samlade in tidigare.
7. Välj **Skicka** för att skicka i din SLA-kreditbegäran.

## <a name="next-steps"></a>Nästa steg

- [Rapportera problem åt din kund](report-problems-on-behalf-of-a-customer.md)
