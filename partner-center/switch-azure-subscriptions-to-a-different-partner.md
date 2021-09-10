---
title: Överföra En Azure-prenumeration till en annan partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Lär dig hur du ändrar Molnlösningsleverantör partner som är associerad med en kunds Azure-prenumerationer.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/21/2021
ms.openlocfilehash: 28e90ec4a699e2d8830f3695a30151e6b00e8cd1
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961006"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-partner-without-converting-them-to-an-azure-plan"></a>Överföra en kunds Azure-prenumerationer till en annan partner utan att konvertera dem till en Azure-plan

**Gäller för:** Partner Center-| Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller:** Global administratör

I den här artikeln beskrivs hur en kund kan överföra en Azure-prenumeration från sin Molnlösningsleverantör (CSP) till en annan CSP.

I det första avsnittet [överföra en Azure-prenumeration](#transferring-azure-subscriptions-to-another-partner)till en annan partner beskrivs hur en kund kan överföra en Microsoft Azure-prenumeration från en Molnlösningsleverantör (CSP) till en annan.

I nästa avsnitt, [Överföra en](#transferring-a-previous-azure-offer-subscription-without-converting-it-to-the-azure-plan)tidigare Azure-erbjudandeprenumeration utan att konvertera den till Azure-planen, beskrivs kortfattat hur den nya Azure-planen introduceras. Sedan beskrivs ett specialfall där vissa prenumerationer till det tidigare Azure-erbjudandet kan överföras till en annan CSP utan att konvertera dem till den nya Azure-planen.

Kunden, den aktuella tjänstleverantören och en ny tjänstleverantör har alla ansvarsområden när en kundprenumeration överförs till [en ny Azure-tjänstleverantör.](#responsibilities-when-transferring-a-customer-subscription-to-a-new-azure-service-provider) En kund bör planera att samarbeta med den aktuella partnern för att övergången ska gå smidigt.

 Information på hög nivå som hjälper Azure-prenumeranter att överföra prenumerationer till och från CSP-partner finns i Överföra Azure-prenumerationer mellan [prenumeranter och molntjänstleverantörer.](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)

Mer information om hur kunder kan ändra sina Azure-prenumerationer från en partner till en annan finns i Överföra en kunds Azure-prenumerationer till en annan [CSP (under en Azure-plan)](/partner-center/transfer-azure-subscriptions-under-azure-plan)

## <a name="prerequisites"></a>Förutsättningar

- En CSP-partner måste ha en återförsäljarrelation med en kund innan en prenumeration kan överföras.  Mer information finns i Så [här begär du en återförsäljarrelation från en kund i Partnercenter.](/partner-center/request-a-relationship-with-a-customer)
- En partner måste vara en direkt provider eller en indirekt leverantör för att överföra en prenumeration.
- Prenumerationer som är kopplade till följande erbjudanden kan inte överföras: Azure-plan, Office 365, Enterprise Mobility Suite och Microsoft Dynamics CRM.
- En kund måste vara i samma land som en partner för att överföra en prenumeration.
- Partner som arbetar i Microsoft Cloud for US Government eller Microsoft Cloud Tyskland måste begära tillstånd att hantera en kunds tjänst eller prenumeration. Mer information finns i [Skaffa behörigheter för att hantera en kunds tjänst eller prenumeration.](/partner-center/customers-revoke-admin-privileges)

## <a name="transferring-azure-subscriptions-to-another-partner"></a>Överföra Azure-prenumerationer till en annan partner

Överföring av en Azure-prenumeration från en CSP-partner till en annan är en process i flera steg som kräver åtgärder från kunden, den aktuella partnern och den nya partnern i olika steg. Följande tabell är avsedd som ett sekvensdiagram för att tydliggöra vem som gör vad och när.

### <a name="responsibilities-when-transferring-a-customer-subscription-to-a-new-azure-service-provider"></a>Ansvarsområden vid överföring av en kundprenumeration till en ny Azure-tjänstleverantör

|Steg  |Kund  |Aktuell partner  |Ny partner  |
|---------|---------|---------|---------|
|1     |[Kunden meddelar Microsoft och den aktuella partnern genom att skriva](#step-1-customer-contacts-current-partner-in-writing)         |         |         |
|2     |         |[Skapa en supportbegäran för att begära överföring](#step-2-current-provider-creates-azure-support-ticket-to-request-a-transfer)        |         |
|3     |         |[Skicka ifyllda överföringsformulär till kunden](#step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer)|         |
|4     |         |[Fullständig ändring av Molnlösningsleverantör formulär](#step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer)       |         |
|5     |[Gransknings-, signerings- & returformulär](#step-5-the-customer-and-new-partner-review--return-the-form)       |         |[Gransknings-, signerings- & returformulär](#step-5-the-customer-and-new-partner-review--return-the-form)         |
|6     |         |[Granskningsformulär och bifoga till tjänstbegäran](#step-6-current-partner-reviews-form-and-attaches-it-to-the-service-request)        |         |
|7     |         |         |[Ta bort gammal partner från konto](#step-7-new-partner-removes-old-partner-from-account)         |
|8     |         |         |[Ta bort inaktuella åtkomstbehörigheter](#step-8-new-partner-removes-outdated-access-permissions)         |

### <a name="steps-for-transferring-a-customer-subscription-to-a-new-azure-service-provider"></a>Steg för att överföra en kundprenumeration till en ny Azure-tjänstleverantör

#### <a name="step-1-customer-contacts-current-partner-in-writing"></a>Steg 1: Kunden kontaktar den aktuella partnern genom att skriva

Kunden påbörjar överföringsprocessen genom att meddela både Microsoft och den aktuella CSP-partnern genom att skriva (det vill säga inte verbalt) om sin begäran om att överföra en prenumeration.

#### <a name="step-2-current-provider-creates-azure-support-ticket-to-request-a-transfer"></a>Steg 2: Den aktuella providern skapar en Azure-supportbegäran för att begära en överföring

Den aktuella partnern skapar en Azure-supportbegäran för att begära en prenumerationsöverföring.

> [!NOTE]
> Det är den aktuella partnerns ansvar att skapa supportbiljetten som initierar överföringsprocessen. Microsoft ingriper inte åt kunden eller den nya partnern.

**Så här skapar du en supportbegäran för att begära en överföring:**

1. I menyn i Partnercenter väljer **du Kunder,** väljer kunden i listan och väljer sedan **Tjänsthantering.**
1. I avsnittet **Supportärenden** väljer du **Nytt ärende** och sedan **Microsoft Azure.**
1. I [Azure Portal](https://portal.azure.com/)väljer du **Ny supportbegäran.**
1. I steg 1 i supportbegäran väljer du Prenumerationshantering som problemtyp, anger det prenumerations-ID som **du** vill överföra och väljer Molnlösningsleverantör som supportplan. 
1. I steg 2 väljer du **C-Minimal påverkan** och **väljer Andra allmänna** frågor som problemtyp.

#### <a name="step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer"></a>Steg 3: Den aktuella partnern fyller i överföringsformuläret och skickar det till kunden

Den aktuella partnern laddar ned och [fyller i Molnlösningsleverantör ,](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)signerar det och skickar det sedan till kunden.

#### <a name="step-4-current-partner-completes-current-partner-fills-in-the-change-of-cloud-solution-provider-form"></a>Steg 4: Den aktuella partnern fyller i formuläret Ändring Molnlösningsleverantör partner

Den aktuella partnern fyller [i Molnlösningsleverantör formulär,](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)signerar det och skickar det till kunden.

En av de uppgifter som behövs för *att slutföra Molnlösningsleverantör* formuläret är:

- **Aktuell partners kontaktinformation och Microsoft-ID** (som finns i menyn i Partnercenter genom att välja Kontoinställningar **> Organisationsprofil**).
- **Kundens Microsoft-ID** (som finns i menyn i Partnercenter genom att välja **Kunder** och sedan expandera kundens lista för att visa sitt Microsoft-ID).
- **Prenumerations-ID** som ska överföras (som finns i menyn  i Partnercenter genom att välja Kunder och sedan expandera kundens lista, välja **Visa** prenumerationer och sedan expandera den valda prenumerationen för att visa prenumerations-ID.

#### <a name="step-5-the-customer-and-new-partner-review--return-the-form"></a>Steg 5: Kunden och den nya partnergranskningen & att returnera formuläret

Arbeta tillsammans, kunden och den nya partnern:

1. Granska formuläret, fyll i information om den nya partnern och signera det.
1. Bekräfta att den nya kunden har ett avtal på plats.
1. Skicka formuläret tillbaka till den aktuella partnern.

#### <a name="step-6-current-partner-reviews-form-and-attaches-it-to-the-service-request"></a>Steg 6: Aktuellt partnergranskningsformulär och bifogar det i tjänstbegäran

När den aktuella partnern får formuläret gör de följande:

- Kontrollera att formuläret innehåller kontaktinformation för båda partneradministratörerna. (Microsoft Support kontaktar båda administratörerna för att verifiera överföringen.)
- Kontrollera att de har alla tre signaturerna och använd sedan alternativet **Fil Upload** för att bifoga det ifyllda formuläret till den befintliga tjänstbegäran. (En Microsoft-supporttekniker kontaktar dem inom åtta timmar för att verifiera kvitto och slutförande.)

#### <a name="step-7-new-partner-removes-old-partner-from-account"></a>Steg 7: Ny partner tar bort gamla partner från kontot

Den nya partnern uppdaterar Azure-prenumerationsinställningarna i PowerShell för att ta bort den gamla partnern från kontot.

> [!NOTE]
> Den första PowerShell-cmdleten kräver kundens **klientorganisations-ID**, som visas i Partnercenter som kundens **Microsoft-ID**. Följande procedur beskriver hur du hittar kundens Microsoft-ID (klientorganisations-ID) som ska användas i cmdleten .

**Så här hittar du en kunds Microsoft-ID (klient-ID) som ska *användas i Anslut-AzAccount* PowerShell-cmdleten**:

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)
1. Välj **Kunder** på menyn.
1. Leta upp kunden i listan som visas.
1. Välj nedåtpilen för att expandera kundens lista. Du ser information om kundens domännamn *och kundens* **Microsoft-ID.**
1. Använd det 16-siffriga **Microsoft-ID:t** i PowerShell-cmdleten som följer den här proceduren.

Den första PowerShell-cmdleten lägger till den nya partnern som återförsäljare på kontot:

```powershell
Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
```

Den andra cmdleten visar rollerna för kontot, inklusive tidigare CSP-partner:

```powershell
Get-AzRoleAssignment
```

#### <a name="step-8-new-partner-removes-outdated-access-permissions"></a>Steg 8: Ny partner tar bort inaktuella åtkomstbehörigheter

   **Så här tar du bort inaktuella åtkomstbehörigheter:**

   1. I menyn i Partnercenter väljer du **Kunder.**
   1. Leta upp kunden i kundlistan.
   1. Dubbelklicka på kundens företagsnamn. Sidan **Kundprenumerationer** visas.
   1. I menyn med kundinformation väljer du **Tjänsthantering.**
   1. Under **Microsoft Azure** väljer du **Microsoft Azure Hanteringsportal**.

## <a name="transferring-a-previous-azure-offer-subscription-without-converting-it-to-the-azure-plan"></a>Överföra en tidigare Azure-erbjudandeprenumeration utan att konvertera den till Azure-planen

Det här avsnittet beskriver kortfattat hur den nya Azure-planen introduceras. Sedan beskrivs ett specialfall där vissa prenumerationer till det tidigare Azure-erbjudandet kan överföras till en annan CSP utan att konvertera dem till den nya Azure-planen.

> [!NOTE]
> Om du vill överföra en kunds Azure-prenumerationer som köptes under det tidigare Azure-erbjudandet till en ny CSP och konvertera dem till *Azure-planen*(som är standardåtgärden) kan du läsa föregående avsnitt Överföra en [*Azure-prenumeration*](#transferring-azure-subscriptions-to-another-partner)till en annan partner och artikeln Överföra en kunds Azure-prenumerationer till en annan [*CSP (under en Azure-plan).*](/partner-center/transfer-azure-subscriptions-under-azure-plan)

### <a name="the-azure-plan-and-the-previous-azure-offer"></a>Azure-planen och det tidigare Azure-erbjudandet

Microsoft introducerade en ny handelsupplevelse, [Azure-planen,](/partner-center/azure-plan-lp)i juli 2021. För att ge partner tid att införliva nya funktioner med sina tjänster och föra över kunder från det tidigare Azure-erbjudandet (MS-AZR-0145p) till Azure-planen fortsätter det tidigare Azure-erbjudandet att vara tillgängligt under en begränsad tid.

Övergången från det tidigare Azure-erbjudandet till Azure-planen sker i tre faser:

**Fas 1:** Sedan Azure-planen introducerades i juli 2021 har alla nya Azure CSP-programkunder lagts till i Azure-planen. Partner kan fortsätta att använda det tidigare Azure-erbjudandet med kunder som redan har köpt det.

**Fas 2:** Den 1 februari 2022 tas incitament och partnermarginaler bort från det tidigare Azure-erbjudandet.

**Fas 3:** Vid en tidpunkt som ännu inte har fastställts kommer det tidigare Azure-erbjudandet att dras tillbaka och kunder som fortfarande har det tidigare Azure-erbjudandet kommer att migreras till Azure-planen. (Partner meddelas om tillbakagången sex månader i förväg.)

### <a name="transferring-subscriptions-without-conversion"></a>Överföra prenumerationer utan konvertering

I det här avsnittet beskrivs det särskilda fallet med överföring av en prenumeration som köptes under det tidigare Azure-erbjudandet till en ny CSP-leverantör, utan att konvertera den till *Azure-planen*.

En kunds prenumeration på det tidigare Azure-erbjudandet kan överföras till en ny CSP-partner utan konvertering till Azure-planen med hjälp av stegen i föregående avsnitt Överföra [Azure-prenumerationer](#transferring-azure-subscriptions-to-another-partner)till en annan partner om:

- Det tidigare Azure-erbjudandet är fortfarande tillgängligt.
- Både den aktuella partnern och den nya partnern har en kund med en prenumeration på det tidigare Azure-erbjudandet.

Om endast den aktuella partnern har en kund med en prenumeration på det tidigare Azure-erbjudandet kan den aktuella partnern använda övergångsverktyget för att flytta kundens prenumeration till den nya partnern samtidigt som den konverteras till den nya Azure-planen.

> [!NOTE]
> Endast partner som har en direktfaktureringsrelation med Microsoft kan komma åt övergångsverktyget. Indirekta återförsäljare måste samarbeta med sina indirekta leverantörer för att använda övergångsverktyget.

## <a name="next-steps"></a>Nästa steg

- [Överföra Azure-prenumerationer](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)
- [Överföra Azure-prenumerationer under en Azure-plan](transfer-azure-subscriptions-under-azure-plan.md)
- Ladda ned [formuläret för överföring av CSP-prenumeration](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)
- Läs mer [om stöd för flera partner](multipartner.md)
- Läs mer [om stöd för flera kanaler](multichannel.md)
