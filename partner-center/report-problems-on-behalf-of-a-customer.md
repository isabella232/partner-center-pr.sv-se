---
title: Rapportera problem för en kunds räkning
ms.topic: how-to
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig när du ska eskalera ett problem med kundtjänsten till Microsoft och hur du kan skapa en supportbiljett för olika typer av Microsoft-tjänster.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f67a3b6a403f09cb773a5ca663d6cf6db1b03e2e
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018126"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Rapportera ett tjänstproblem åt en kund – inklusive när och hur du gör det

**Gäller för**

- Välkommen till Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller**

- Global administratör

Om kunden har ett tjänstproblem som du inte kan lösa och som uppfyller kriterierna som beskrivs i Eskalera problem till [Microsoft](escalate-problems-to-microsoft.md)kan din indirekta leverantör skapa en supportbiljett åt dem. Den här processen är också användbar för att eskalera faktureringsproblem eller tvister och för bedrägeriproblem.

## <a name="submit-a-service-request-for-a-customer"></a>Skicka en tjänstbegäran för en kund

1. På menyn i Partnercenter under CSP väljer du **Kunder**

2. På sidan Kunder väljer eller söker du efter den kund som du vill ha
    
3. Välj Tjänstförfrågningar på **kundmenyn**

4. I **listrutan Ny** begäran väljer du **antingen Azure** eller **Office 365, Dynamics 365, Enterprise Mobility Suite.** Du omdirigeras till antingen Microsoft Azure-portalen eller administrationscentret för Office 365.

>[!NOTE]
>Support operations-partner som gör transaktioner med Dynamics 365 i CSP krävs för att upprätthålla ett supportavtal med ASfP-plan (Advanced Support for Partner) eller högre. Det här supportavtalet krävs för att skicka Dynamics 365-incidenter åt en CSP-kund. [Läs mer](https://partner.microsoft.com/support/partnersupport) om alternativen för supportavtal.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Tänk på följande när du behöver skapa en tjänstbegäran för din kund i Azure:
>
>- För att du som indirekt återförsäljare ska kunna skapa tjänstbegäranden för din kund i Azure måste din indirekta leverantör ge dig åtkomst till kundens Azure-konto. Detta skiljer sig från administration för kunders räkning för Office 365.
>
>- Supportadministratören i Partnercenter kan inte skapa tjänstbegäranden i Azure-tjänstportalen, men det de kan göra är att skapa en supportgrupp i Azure-tjänstportalen och ge gruppen behörighet att logga supportförfrågningar.

1. Välj **Ny supportbegäran**.

2. Fyll i supportbegäran med lämplig information och välj sedan **Skapa:**

   - I avsnittet **Grundläggande i** supportbegäran ser du till att Molnlösningsleverantör **i** **fältet Supportplan.**

   - I **avsnittet Kontaktinformation** i supportbegäran anger du din information, inte kundens information.

3. Senare kan du granska kundens tjänstbegäranden i Microsoft Azure-portalen genom att **välja Hantera supportbegäranden.**

Du kan behöva skapa en supportbegäran för en kund när du inte har administratörsbehörighet för den kunden. Detta kan inträffa i ett av två scenarier:

- Du har inte begärt administratörsbehörighet när du först etablerade relationen.
- Du hanterar bara en kunds Azure-prenumerationer, så att du inte har administratörsbehörighet.
 
I något av dessa fall kan du använda följande procedur för att skapa en supportbegäran. 

1. Kopiera kundens domännamn från kontosidan i Partnercenter.

2. Gå till https://portal.azure.com/ [customerdomainname]. 

3. Välj den Azure-prenumeration som kräver support.

4. Välj **Ny supportbegäran** och följ sedan anvisningarna för att skapa begäran. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. I avsnittet **Skapa en tjänstbegäran** väljer du lämplig supportkategori. Du kan behöva välja **Mer... om** du vill visa fler artiklar.

2. Fyll i formuläret för tjänstbegäran och välj **Skicka**.

   > [!TIP]
   > Se till att inkludera dina kontaktuppgifter, inte kundens.

3. Senare granskar du kundens tjänstbegäranden genom att gå till Administrationscenter för Office 365 och välja **Visa alla supportärenden.**

### <a name="support-for-commercial-marketplace-products"></a>Stöd för produkter på den kommersiella marknadsplatsen

Microsoft tillhandahåller inte produktsupport för produkter från den kommersiella marknadsplatsen. Du måste kontakta den oberoende programvaruleverantören (ISV) som publicerade produkten för att få support.

Så här hittar du ISV:ens kontaktinformation:

1.  På Sidan **Marketplace** väljer du den produkt som du behöver hjälp med.

2.  På produktsidan hittar du kontaktinformation för supporten. Detta kan vara ett eller flera av följande alternativ:

    - En länk till en support-startpunkt på ISV:s webbplats
    - Ett e-postmeddelande för support
    - Ett telefonnummer till supportkontakten

## <a name="faq"></a>Vanliga frågor

Se följande vanliga frågor och svar om tjänstbegäranden som du kan skicka för en kunds räkning. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>Vad ingår som en del av supportberättigandet?

Tjänstbegäranden ska arkiveras via Partnercenter. De är tillgängliga för Azure, Microsoft Office 365, Microsoft Dynamics CRM Online och Enterprise Mobility Suite. Som partner som deltar i Molnlösningsleverantör program kan du förvänta dig prioritetssvarstid för dina större problem.

Stöd för din egen partnerklientorganisation ingår inte som en del av CSP-supportförmånen. Office 365, Microsoft Dynamics CRM Online och Enterprise Mobility Suite debiterar dock inte en separat prenumerationsavgift för support för partner eller kunder. Azure debiterar en avgift, men om du är berättigad till Signature Cloud Support eller andra Microsoft Partner Network-förmåner (MPN) kan du använda dessa förmåner för att betala avgiften.

Den här förmånen gäller för alla partner som deltar i Molnlösningsleverantör-programmet, oavsett om de har betalats eller under en utvärderingsperiod. Support för fakturering och prenumerationshantering ingår också som en kostnadsfri komponent i det här paketet.

### <a name="how-quickly-will-i-get-an-initial-response"></a>Hur snabbt får jag ett första svar?

Våra första svarstider beror på allvarlighetsgraden för den incident som skickats. Problemets allvarlighetsgrad bestäms av din indikation på affärspåverkan när du skickar en tjänstbegäran.

Inledande svarstider för **tekniska felkorrigeringar:**

- Kritisk påverkan (allvarlighetsgrad A): Två timmar (betydande förlust eller försämring av tjänster. Produktionstjänster nere.)
- Måttlig påverkan (allvarlighetsgrad B): Fyra timmar (måttlig förlust eller försämring av tjänster. Produktionstjänster påverkas delvis.)
- Minimal påverkan (allvarlighetsgrad C): Åtta timmar (minimal förlust eller försämring av tjänster. Tjänster som fortfarande är tillgängliga eller icke-produktionstjänster som påverkas.)

Inledande svarstider är endast för engelsktalande support. Stöd för lokala språk tillhandahålls under arbetstid.
För incidenter som faller inom gränserna för supporträttigheterna men inte betraktas som incidenter som åtgärdas kan den inledande svarstiden vara upp till en arbetsdag.

### <a name="can-i-submit-a-service-request-by-phone"></a>Kan jag skicka en tjänstbegäran via telefon?

Nej, telefonsupport erbjuds inte för det här programmet.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>Vad händer om jag loggar in på Azure Portal och kringgår Partnercenter?

Om du loggar in Microsoft Azure-portalen direkt visar du mitten i din egen kontext, inte en kunds kontext. Därför bör du bara logga in direkt på Microsoft Azure-portalen när du skapar en tjänstbegäran för dina egna prenumerationer.

Supporträttigheterna för CSP-programmet ger inte support för din egen partnerprenumeration. Därför måste du ange en giltig supportplan när du skapar en tjänstbegäran som gäller din egen partnerprenumeration. Exempel är MPN-kontrakts-ID, Premier eller ett Azure-supportavtal. Mer information finns i vanliga Azure Support [vanliga frågor och svar.](https://go.microsoft.com/fwlink/?LinkId=717532)

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>Vad händer om jag loggar in på administrationscenterportalen för Office 365 och kringgår Partnercenter?

Om du loggar in direkt i administrationscentret för Office 365 visar du mitten i din egen kontext, inte en kunds kontext. Därför bör du bara logga in direkt i Administrationscenter för Office 365 när du skapar en tjänstbegäran för dina egna prenumerationer.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>Hur gör jag för att du ytterligare stöd för Dynamics 365?

Om du har problem som rör: Dynamics 365-prenumerationsplan, licensiering, fakturering, Finance & Operations, Dynamics 365-produktlicenser eller om du behöver ytterligare teknisk support:
 
Kontakta [Dynamics-supporten](/dynamics365/customer-engagement/admin/contact-technical-support)

## <a name="next-steps"></a>Nästa steg

- [Ge support till dina kunder](customer-support.md)
- [Kontrollera tjänststatus](check-service-health.md)
