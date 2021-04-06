---
title: Rapportera problem för en kunds räkning
ms.topic: how-to
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig när du ska eskalera ett kund service problem till Microsoft och hur du kan använda ett support ärende för olika typer av Microsoft-tjänster.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 80c617a97575fea3003ea8652d48396412033cc7
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441956"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Rapportera ett tjänst problem för en kunds räkning, inklusive när och hur du gör det

**Gäller för**

- Välkommen till Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller**

- Indirekt Provider

Om kunden drabbas av ett tjänst problem som du inte kan lösa, och som uppfyller de kriterier som beskrivs i [eskalera problem till Microsoft](escalate-problems-to-microsoft.md), kan din indirekta leverantör ge dem ett support ärende. Den här processen är också användbar för att eskalera fakturerings problem eller tvister och för bedrägerier.

## <a name="submit-a-service-request-for-a-customer"></a>Skicka en tjänstbegäran för en kund

1. Från menyn Partner Center under KRYPTOGRAFIPROVIDER väljer du **kunder**

2. På sidan kunder väljer eller söker du efter den kund du vill
    
3. Från menyn kund väljer du **tjänst begär Anden**

4. Välj antingen **Azure** eller **Office 365, Dynamics 365, Enterprise Mobility Suite** från List menyn **ny begäran** . Du omdirigeras till antingen Microsoft Azure-portalen eller administrations centret för Office 365.

>[!NOTE]
>Support åtgärds partner som samverkar med Dynamics 365 i CSP krävs för att upprätthålla ett support avtal med en ASfP-plan (Advanced support for partner) eller högre. Detta support avtal krävs för att skicka Dynamics 365-incidenter för en CSP-kunds räkning. [Läs mer](https://partner.microsoft.com/support/partnersupport) om alternativen för support avtal.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> När du behöver skapa en tjänstbegäran för din kund i Azure bör du vara medveten om följande:
>
>- För dig, som den indirekta åter försäljaren, för att skapa tjänst begär Anden för din kund i Azure, måste den indirekta leverantören ge dig åtkomst till kundens Azure-konto. Detta skiljer sig från att administrera kundernas räkning för Office 365.
>
>- Även om supportavdelningen i Partner Center inte kan skapa tjänst begär anden i Azure Service Portal, vad de kan göra är att skapa en support grupp i Azure Service Portal och ge gruppen behörighet att logga support förfrågningar.

1. Välj **Ny supportbegäran**.

2. Fyll i support förfrågan med lämplig information och välj sedan **skapa**:

   - I avsnittet **grundläggande** information om support begär du att välja **Cloud Solution Provider** i fältet **Support plan** .

   - I avsnittet **kontakt** information i support förfrågan anger du din information, inte kundens information.

3. Granska sedan kundens tjänst begär anden i Microsoft Azure-portalen genom att välja **Hantera support förfrågningar**.

Du kan behöva skapa en support förfrågan för en kund när du inte har administratörs behörighet för den kunden. Detta kan inträffa i något av två fall:

- Du har inte begärt administratörs behörighet när du först upprättade relationen.
- Du hanterar bara en kunds Azure-prenumerationer, så du har inte administratörs behörighet.
 
I något av dessa fall kan du använda följande procedur för att skapa en support förfrågan. 

1. Kopiera kundens domän namn från deras konto sida i Partner Center.

2. Gå till https://portal.azure.com/ [customerdomainname]. 

3. Välj den Azure-prenumeration som kräver support.

4. Välj **ny supportbegäran** och följ sedan anvisningarna för att skapa begäran. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. Välj lämplig support kategori i avsnittet **skapa en tjänstbegäran** . Du kan behöva välja **fler...** om du vill visa fler artiklar.

2. Slutför formuläret för tjänstbegäran och välj **Skicka**.

   > [!TIP]
   > Se till att ta med din kontakt information, inte kundens.

3. Granska din kunds tjänst begär Anden senare genom att gå till administrations centret för Office 365 och välja **Se alla support ärenden**.

### <a name="support-for-commercial-marketplace-products"></a>Stöd för kommersiella Marketplace-produkter

Microsoft tillhandahåller inte produkt support för produkter på kommersiella platser. Du måste kontakta den oberoende program varu leverantören (ISV) som publicerade produkten för att få support.

Så här hittar du ISV: s kontakt information:

1.  På **Marketplace** -sidan väljer du den produkt du behöver hjälp med.

2.  På produktens sida hittar du support kontakt information. Detta kan vara ett eller flera av följande alternativ:

    - En länk till en support start punkt på ISV-webbplatsen
    - Ett support-e-postmeddelande
    - Telefonnummer till support kontakt

## <a name="faq"></a>Vanliga frågor

Se följande vanliga frågor om tjänst begär Anden som du kan skicka till en kunds räkning. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>Vad ingår som en del av support rättigheten?

Tjänst begär Anden bör arkiveras via partner Center. De är tillgängliga för Azure, Microsoft Office 365, Microsoft Dynamics CRM Online och Enterprise Mobility Suite. Som partner som ingår i Cloud Solution Provider-programmet kan du förväntar dig svars tiden för dina huvud problem.

Support för din egen partner klient ingår inte som en del av support förmånerna för CSP. Office 365, Microsoft Dynamics CRM Online och Enterprise Mobility Suite debiterar dock inte en separat support prenumerations avgift för partner och kunder. Azure debiterar en avgift, men om du är berättigad till Signature Cloud Support eller andra Microsoft Partner Network (MPN)-förmåner kan du använda dessa för att betala avgiften.

Den här förmånen gäller alla partner som deltar i Cloud Solution Provider-programmet, vare sig det betalas eller en utvärderings period. Support för fakturering och prenumerations hantering ingår också som en kostnads fri komponent i det här paketet.

### <a name="how-quickly-will-i-get-an-initial-response"></a>Hur snabbt får jag ett första svar?

Våra första svars tider beror på allvarlighets graden för den inskickade incidenten. Problemets allvarlighets grad bestäms av ditt val av affärs påverkan när du skickar en tjänstbegäran.

Första svars tider för **tekniska brotts lösa incidenter**:

- Kritisk påverkan (allvarlighets grad A): två timmar (betydande förlust eller försämring av tjänster. Produktions tjänster är nere.)
- Måttlig påverkan (allvarlighets grad B): fyra timmar (måttlig förlust eller försämring av tjänster. Produktions tjänster som påverkas delvis.)
- Minimal påverkan (allvarlighets grad C): åtta timmar (minimal förlust eller försämring av tjänster. Tjänster som fortfarande är tillgängliga eller icke-produktions tjänster påverkas.)

De första svars tiderna är för engelska och stöder endast support. Support för lokalt språk tillhandahålls under kontors tid.
För incidenter som faller inom gränserna för support rättigheten men inte betraktas som brotts lösa incidenter kan den första svars tiden vara upp till en arbets dag.

### <a name="can-i-submit-a-service-request-by-phone"></a>Kan jag skicka en service förfrågan per telefon?

Nej, telefon support erbjuds inte för det här programmet.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>Vad händer om jag loggar in på Azure Portal och kringgår Partner Center?

Om du loggar in på Microsoft Azure-portalen direkt visas Center i ditt eget sammanhang, inte i kundens sammanhang. Därför bör du bara logga in direkt i Microsoft Azure-portalen när du skapar en tjänstbegäran för dina egna prenumerationer.

Ditt CSP-program stöder rättigheten ger inte stöd för din egen partner prenumeration. Därför måste du ange en giltig support Plans rättighet när du skapar en tjänstbegäran som berör din prenumeration på din egen partner. Exempel innefattar MPN kontrakts-ID, Premier eller ett support avtal för Azure. Mer information finns i [vanliga frågor och svar om support för Azure](https://go.microsoft.com/fwlink/?LinkId=717532).

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>Vad händer om jag loggar in på Office 365 administrations Center-portalen och kringgår Partner Center?

Om du loggar in på administrations centret för Office 365 direkt visas Center i ditt eget sammanhang, inte en kunds sammanhang. Det är därför du bör bara logga in direkt i administrations centret för Office 365 när du skapar en tjänstbegäran för dina egna prenumerationer.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>Hur gör jag för att få ytterligare stöd för Dynamics 365?

Om du har problem som rör: Dynamics 365 planera prenumerationer, licensiering, fakturering, ekonomi & åtgärder, Dynamics 365 produkt licenser eller om du behöver ytterligare teknisk support:
 
Kontakta [Dynamics support](/dynamics365/customer-engagement/admin/contact-technical-support)

## <a name="next-steps"></a>Nästa steg

- [Ge support till dina kunder](customer-support.md)
- [Kontrollera tjänststatus](check-service-health.md)
