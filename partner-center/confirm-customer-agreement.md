---
title: Bekräfta kundens samtycke till Microsofts kundavtal
description: Leverantörer av moln lösningar (CSP) behöver bekräfta kund godkännande av Microsofts kund avtal innan de beställer Microsoft-tjänster för kunder.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 05/05/2020
ms.openlocfilehash: 423cf1aab281ad8e77e03aa386b43360e1b99b3c
ms.sourcegitcommit: 6b03ff400d1350db9696f9b457fcfe710310c5d3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/03/2020
ms.locfileid: "96570577"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a>Bekräfta kund godkännande av Microsofts kund avtal i CSP partner-programmet

**Gäller för**

- Partnercenter
- Microsoft 365 administrations Center

**Lämpliga roller**

- Administratörs agent
- Försäljnings agent

Den 1 oktober 2019 introducerade Microsoft **kund avtalet** till CSP-programmet för att ersätta Microsoft Cloud avtalet. Läs ytterligare [vägledning](indirect-reseller-tasks-in-partner-center.md) för indirekta åter försäljare. För att under lätta migreringen av partner till det nya avtalet, finns båda avtalen i CSP-programmet fram till den 31 januari 2020. Från och med den 1 februari 2020 ersatte Microsofts kund avtal Microsoft Cloud avtalet.

Kunder har två alternativ för att godkänna Microsofts kund avtal. 

**Alternativ 1**: partner attestering för kund godkännande – partner kan bekräfta kund acceptansen med hjälp av Partner Center API/SDK eller via instrument panelen för partner Center.

**Alternativ 2**: Kunddirekt godkännande – partner kan bjuda in kunden via en URL för att granska och godkänna avtalet i Microsoft 365 administrations centret.

## <a name="access-microsoft-customer-agreement-template"></a>Få åtkomst till Microsofts kundavtals mall

Du kan manuellt hämta den senaste versionen av Microsoft kund avtals mal len [härifrån.](https://aka.ms/customeragreement) Microsofts kund avtal är landsspecifika. När du begär Microsofts kund avtals mall måste du välja rätt land baserat på kundens plats.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Alternativ 1: bekräfta kund godkännande i Partner Center

Partner kan bekräfta kund godkännande av Microsofts kund avtal i Partner Center för nya och befintliga kunder. Åter försäljare kan inte attestera sina kunders räkning och behöver arbeta med sin indirekta leverantör för att få attesteringen slutförd.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Bekräfta kund godkännande för nya kunder

När du skapar en ny kund klient i Partner Center kan du använda följande steg för att bekräfta kundens godkännande av Microsofts kund avtal. Du måste vara administratörs agent eller försäljnings agent för att kunna utföra dessa steg.

1. Välj **kunder** och sedan **ny kund**.

2. Under **konto information** anger du information för företaget och den primära kontakten.

3. Under **Microsoft-avtal** markerar du kryss rutan för att bekräfta att kunden har godkänt Microsofts kund avtal.

4. Ange ett datum under **avtalets godkännande datum**. Du kan inte ange ett framtida datum.

5. Kontrol lera att den primära användar kontakt informationen som visas är korrekt. Om den är felaktig väljer du **Uppdatera** och anger korrekt information för den person som har godkänt avtalet.

6. Välj **Nästa** för att fortsätta skapa kund klienten.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Ny kund":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Bekräfta kund godkännande för befintliga kunder

Du måste vara administratörs agent eller försäljnings agent för att göra detta:

1. Välj **Kunder**. Sök efter och välj kunden.

2. Välj **konto information**.

3. Under **Microsofts kund avtal** väljer du **Uppdatera**.

4. Ange **förnamn**, **efter namn**, **e-postadress** och **telefonnummer** (valfritt) för den person som har godkänt avtalet. Ange ett datum under **avtalets godkännande datum**. Du kan inte ange ett framtida datum.

5. Välj **Spara** och fortsätt.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Befintlig kund":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Hämta bekräftelse av kund godkännande

Du kan hämta en bekräftelse på att en befintlig kund har godkänt Microsofts kund avtal med hjälp av följande steg. Du måste vara administratörs agent eller försäljnings agent för att göra detta.

1. Välj **kunder** och leta upp och välj den kund som du vill se.

2. Välj **konto information**.

3. Under **Microsofts kund avtal** kan du Visa om bekräftelsen har eller inte har tillhandahållits av den här kunden.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Bekräfta kund godkännande med partner Center API/SDK

Du kan använda Partner Center API/SDK för att bekräfta kund godkännande av Microsofts kund avtal. Mer information om API/SDK finns i:

- [Hämta avtals-metadata för Microsofts kund avtal](/partner-center/develop/get-customer-agreement-metadata)

- [Bekräfta kund godkännande av Microsofts kund avtal](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Få bekräftelse på kund godkännande av Microsofts kund avtal](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Hämta en nedladdnings länk för Microsofts kund avtals mall](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Alternativ 2: kund godkännande i Microsoft 365 administrations Center

Partner kan bjuda in nya och befintliga kunder via en URL för att granska och godkänna avtalet i Microsoft 365 administrations centret. I följande avsnitt visas hur du:

- Skapa en ny kund och Bjud in kunden att granska och godkänna avtalet.

- Bjud in en ny kund att granska och godkänna åter försäljarens relation och avtal.

- Bjud in en befintlig kund för att granska och godkänna avtalet.

>[!NOTE]
> Du kan använda [partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) för att hämta statusen för kundens direkta godkännande av Microsofts kund avtal.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Skapa en ny kund och Bjud in kunden att granska och godkänna avtalet

Använd följande steg för att skapa en ny kund i Partner Center och sedan bjuda in dem att granska och godkänna Microsofts kund avtal i Microsoft 365 administrations Center.

1. Välj **Lägg till kund** på fliken **kunder** i Partner Center.

2. Under **konto information** anger du information om den nya kunden i alla obligatoriska fält, inklusive kundens företags namn och primär kontakt.

3. Under **kund avtal** väljer du det första alternativet. **kunden uppmanas att godkänna Microsofts kund avtal i Microsoft 365 administrations Center**. Fyll i alla andra obligatoriska fält på sidan.

4. Välj **Nästa: granska** och fortsätt sedan stegen för att skapa kund klienten. 

>[!NOTE] 
>Nya kunder kan inte göra ett nytt inköp förrän de accepterar Microsofts kund avtal.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Skapa ny kund":::

5. När du når **bekräftelse** skärmen i det nya kund arbets flödet sparar du kundens autentiseringsuppgifter. Du måste ange autentiseringsuppgifterna för din kund senare.

6. Utanför Partner Center skapar och skickar du ett e-postmeddelande som bjuder in kunden att godkänna Microsofts kund avtal i Microsoft 365 administrations Center. Se till att ta med dessa objekt i e-postmeddelandet:

   - En länk till denna [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (inloggning krävs)

   - Kundens autentiseringsuppgifter som du sparade i steg 5.

7. Kunden får sedan e-postinbjudan från partnern och välja [URL: en](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Kunden loggar in i Microsoft 365 administrations Center med hjälp av de kundautentiseringsuppgifter som tidigare togs emot från partnern.

9. Kunden kontrollerar sedan rutan för att godkänna Microsofts kund avtal.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Bjud in en ny kund att granska och godkänna åter försäljarens relation och Microsofts kund avtal 

Använd följande steg för att bjuda in en ny kund att granska och godkänna åter försäljarens relation och Microsofts kund avtal. 

1. På fliken **kunder** i Partner Center väljer du **begär en åter försäljares Relations** länk. 

2. En mall för automatisk e-post kommer att skapas, inklusive text och en parametriserad URL som leder kunden till Microsoft 365 administrations Center.

3. Du kan anpassa den automatiskt genererade e-postmallen och sedan välja **Kopiera till Urklipp** eller **Öppna i e-post**.

4. Använd den här e-postmallen för att bjuda in kunden att acceptera **åter försäljarens Relations** förfrågan och **Microsofts kund avtal**. (Obs! i e-postinbjudanen ser du till att partnern även innehåller den URL som angavs automatiskt samt de autentiseringsuppgifter för kunden som nyligen har skapats.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="skapa en relation":::

5. Kunden tar emot inbjudan via e-post och klickar på URL: en för parametern. 

6. Kunden använder autentiseringsuppgifter från partnern i e-postmeddelandet för att logga in på Microsoft 365 administrations Center.

7. Kunden kontrollerar rutan för att godkänna **åter försäljarens relation** och **Microsofts kund avtal**. 

8. Inom samma URL kan kunden se en lista över olika partners som de arbetar med. De kan välja en partner för att se information.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Godkänna avtal":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Bjud in en befintlig kund för att granska och godkänna avtalet

Använd följande steg för att bjuda in en befintlig kund att granska och godkänna Microsofts kund avtal. 

1. Skapa kund-e-postmeddelandet med den inbäddade URL: en som bjuder in kunden att godkänna Microsofts kund avtal.

2. Kunden får inbjudan via e-post och klickar på [URL: en](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Kunden anger sina autentiseringsuppgifter i Microsoft 365 administrations Center.

4. Kunden söker i rutan om att godkänna Microsofts kund avtal. 

5. I samma URL kan kunden se den konsoliderade listan över olika partners som de arbetar med. De kan välja en partner för att se information.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="kund":::

>[!NOTE]
>I vissa fall kanske kunderna inte kan acceptera Microsofts kund avtal direkt. Mer information om de här situationerna finns i [två scenarier där du behöver intyga för kundens räkning](attest-acceptance-customer-agreement.md).

### <a name="historical-timeline-details"></a>Information om historisk tids linje

| Datum | Gränser | Information |
|------------|------------|--------------------------------|
|01 augusti 2019| UX-förhandsgranskning som är tillgänglig i sandbox| Partner kan bekräfta kund godkännande av Microsofts kund avtal med hjälp av Partner Center-instrumentpanelen i sand Box miljön för KRYPTOGRAFI. Partner med åtkomst till CSP sandbox-miljön för hands versions ändringar av användar upplevelsen. Partner utan sandbox-åtkomst kan lära sig mer om ändringarna i det här avsnittet.|
|September 03 2019|API Preview är tillgängligt i begränsat läge.|Partner kan bekräfta kund godkännande av Microsofts kund avtal med hjälp av API för partner Center i sand Box miljö. API-partner kan använda den här möjligheten för att förhandsgranska API-ändringar och börja arbeta med API-integrering för att stödja det nya avtalet.|
|20 september 2019|.NET SDK-förhands granskning är tillgänglig i begränsat läge.|Partner kan bekräfta kund godkännande av Microsofts kund avtal med partner Center .NET SDK i sand Box miljö. API-partner kan använda den här möjligheten för att förhandsgranska .NET SDK-ändringar och börja arbeta med API-integrering för att stödja det nya avtalet.|
|01 oktober 2019|Microsofts kund avtal finns i produktion|Microsoft presenterar Microsofts kund avtal till CSP-programmet för att ersätta Microsoft Clouds avtalet. Partner kan bekräfta kund godkännande av Microsofts kund avtal med hjälp av Partner Center-instrumentpanelen och API: et i produktionen. Microsoft Cloud avtalet stöds fortfarande i CSP-partnerprogram. Partner uppmanas dock att börja migrera till Microsofts kund avtal. Nya inköps-och licens antal ändringar i befintliga prenumerationer kräver partner bekräftelse av antingen Microsofts kund avtal eller Microsoft Cloud avtal. Vissa nya erbjudanden (till exempel den nya Azure-prenumerationen) kräver att du bekräftar Microsofts kund avtal.|
|31 januari 2020|Microsoft Cloud avtalet har tagits bort från produktionen|Microsoft Cloud avtalet godkänns inte längre i CSP-partner programmet. Nya köp-och licens antal ändringar i befintliga prenumerationer kräver att partnern tillhandahåller en bekräftelse på Microsofts kund avtal. Detta krav gäller för nya kunder och befintliga kunder som tidigare har godkänt Microsoft Cloud avtalet.|
|3 februari 2020|Partner har nu möjlighet att bjuda in kunden via en URL för att granska och godkänna avtalet i autentiserade Microsoft 365 administrations Center. | Kunden kan godkänna Microsofts kund avtal i Microsoft 365 administrations Center. Kundens direkta godkännande av avtalet i Microsoft 365 Admin Center bekräftar godkännande av villkor. 