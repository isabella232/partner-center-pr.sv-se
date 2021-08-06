---
title: Så här bekräftar du att kunden har godkänt Microsoft-kundavtal till CSP-programmet
description: Molnlösningsleverantör (CSP)-partner måste bekräfta kundens godkännande av Microsoft-kundavtal innan de beställer Microsoft-tjänster för kunder.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ed3b888791dad1e875db64b7ccbe20e7b0a8b4bbd71fb7c83cc677ee2d5f2d3a
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115680108"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Så här bekräftar du att kunden har godkänt Microsoft-kundavtal till CSP-programmet

**Lämpliga roller:** Administratörsagent | Försäljningsagent


Kunder har två alternativ för hur de accepterar Microsoft-kundavtal.

**Alternativ 1:** Partner attestation av kundgodkännande – Partner kan bekräfta kundens godkännande via Partner Center API/SDK eller via instrumentpanelen i Partnercenter.

**Alternativ 2:** Direkt godkännande av kund – Partner kan bjuda in kunden via en URL för att granska och godkänna avtalet i Microsoft 365 Admin Center.

## <a name="access-microsoft-customer-agreement-template"></a>Åtkomst Microsoft-kundavtal mall

Du kan ladda ned den senaste versionen av Microsoft-kundavtal [här.](https://aka.ms/customeragreement) Den Microsoft-kundavtal är landsspecifik. När du Microsoft-kundavtal mallen måste du välja rätt land baserat på kundens plats.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Alternativ 1: Bekräfta kundens godkännande i Partnercenter

Direktfaktureringspartner kan bekräfta att kunden godkänner Microsoft-kundavtal i Partnercenter för nya och befintliga kunder. Indirekta återförsäljare kan inte intyga för sina kunders räkning och behöver samarbeta med sin indirekta leverantör för att slutföra attestering.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Bekräfta kundens godkännande för nya kunder

När du skapar en ny kundklientorganisation i Partnercenter använder du följande steg för att bekräfta kundens godkännande av Microsoft-kundavtal. Du måste vara administratörsagent eller försäljningsagent för att utföra de här stegen.

1. Välj **Kunder** och sedan **Ny kund.**

2. Under **Kontoinformation** anger du information för företaget och dess primära kontakt.

3. Under **Microsoft-avtal** markerar du rutan för att intyga att kunden har accepterat Microsoft-kundavtal.

4. Under **Godkännandedatum för avtalet** anger du lämpligt datum. Du kan inte ange detta till ett framtida datum.

5. Kontrollera att den primära användarens kontaktuppgifter visas korrekt. Om det är felaktigt väljer du **Uppdatera** och anger korrekt information för den person som godkände avtalet.

6. Välj **Nästa för** att fortsätta att skapa kundklientorganisationen.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Ny kund.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Bekräfta kundgodkännande för befintliga kunder

Du måste vara administratörsagent eller försäljningsagent för att göra detta:

1. Välj **Kunder**. Leta upp och välj kunden.

2. Välj **Kontoinformation.**

3. Under **Microsoft-kundavtal** väljer du **Uppdatera**.

4. Ange **förnamn,** **efternamn,** **e-postadress** **och Telefon (valfritt)** för den person som godkände avtalet. Under **Godkännandedatum för avtalet** anger du lämpligt datum. Du kan inte ange detta till ett framtida datum.

5. Välj **Spara** och fortsätt.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Befintlig kund.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Hämta bekräftelse av kundgodkännande

Använd följande steg för att hämta en bekräftelse Microsoft-kundavtal en befintlig kund har accepterat Microsoft-kundavtal. Du måste vara administratörsagent eller försäljningsagent för att göra detta.

1. Välj **Kunder** och leta upp och välj sedan den kund som du vill se.

2. Välj **Kontoinformation.**

3. Under **Microsoft-kundavtal** visar du om en bekräftelse har eller inte har tillhandahållits av den här kunden.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Bekräfta kundgodkännande med partnercenter-API/SDK

Du kan använda Partner Center API/SDK för att bekräfta kundens godkännande av Microsoft-kundavtal. Mer information om API/SDK finns i:

- [Hämta avtalsmetadata för Microsoft-kundavtalet](/partner-center/develop/get-customer-agreement-metadata)

- [Bekräfta kundgodkännande av Microsoft-kundavtal](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Få bekräftelse på kundgodkännande av Microsoft-kundavtal](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Hämta en nedladdningslänk för Microsoft-kundavtal mallen](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Alternativ 2: Kundgodkännande i Microsoft 365 Admin Center

Partner kan bjuda in nya och befintliga kunder, via en URL, för att granska och godkänna avtalet i Microsoft 365 Admin Center. I följande avsnitt visas hur du:

- Skapa en ny kund och bjud in kunden att granska och godkänna avtalet.

- Bjud in en ny kund att granska och godkänna återförsäljarrelationen och avtalet.

- Bjud in en befintlig kund att granska och godkänna avtalet.

>[!NOTE]
> Du kan använda [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) för att få status för en kunds direkta godkännande av Microsoft-kundavtal.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Skapa en ny kund och bjud in kunden att granska och godkänna avtalet

Använd följande steg för att skapa en ny kund i Partnercenter och sedan bjuda in dem att granska och godkänna Microsoft-kundavtal i Microsoft 365 Admin Center.

1. På fliken **Kunder** i Partnercenter väljer du Lägg **till kund.**

2. Under **Kontoinformation** anger du information om den nya kunden i alla obligatoriska fält, inklusive kundens företagsnamn och primära kontakt.

3. Under **Kundavtal** väljer du **Customer will be to accept the Microsoft-kundavtal in Microsoft 365 Admin Center**. Fyll i alla andra obligatoriska fält på sidan.

4. Välj **Nästa: Granska och** fortsätt sedan stegen för att skapa kundklientorganisationen. 

>[!NOTE] 
>Nya kunder kan inte göra ett köp förrän de accepterar Microsoft-kundavtal.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Skapa en ny kund.":::

5. När du når **bekräftelseskärmen i** det nya kundarbetsflödet sparar du kundens autentiseringsuppgifter. Du måste ge dessa autentiseringsuppgifter till kunden senare.

6. Utanför Partnercenter skapar och skickar du ett e-postmeddelande som uppmanar kunden att godkänna Microsoft-kundavtal i Microsoft 365 Admin Center. Se till att inkludera dessa objekt i e-postmeddelandet:

   - En länk till [den här URL:en](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (inloggning krävs)

   - Kundens autentiseringsuppgifter som du sparade i steg 5.

7. Kunden får sedan e-post inbjudning från partnern och väljer [URL:en](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Kunden loggar in på Microsoft 365 Admin Center med de kundautentiseringsuppgifter som du angav.

9. Kunden kontrollerar kryssrutan för att godkänna Microsoft-kundavtalet.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Bjud in en ny kund att granska och godkänna återförsäljarrelationen och Microsoft-kundavtal 

Använd följande steg för att bjuda in en ny kund att granska och godkänna återförsäljarrelationen och Microsoft-kundavtal. 

1. På fliken **Kunder** i Partnercenter väljer du Länken **Begär en återförsäljarrelation.** 

2. En automatisk e-postmall genereras, inklusive text och en parametriserad URL som dirigerar kunden till Microsoft 365 Admin Center.

3. Du kan anpassa den automatiskt genererade e-postmallen och sedan välja **Kopiera till Urklipp eller** Öppna i **e-post**.

4. Använd den här e-postmallen för att bjuda in kunden **att** godkänna begäran om återförsäljarrelation och **Microsoft-kundavtal**. (Obs! I e-postbjudan kontrollerar du att partnern även innehåller den URL som angavs automatiskt samt de kundautentiseringsuppgifter som nyligen skapades.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="skapa en relation.":::

5. Kunden får inbjudan via e-post och klickar på den parametriserade URL:en. 

6. Kunden använder de autentiseringsuppgifter som du anger i e-postmeddelandet för att logga Microsoft 365 Admin Center.

7. Kunden kontrollerar kryssrutan för att godkänna **återförsäljarrelationen** och **Microsoft-kundavtal**. 

8. Inom samma URL kan kunden se en samlad lista över olika partner som de arbetar med. De kan välja en partner för att se information.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Godkänn avtalet.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Bjud in en befintlig kund att granska och godkänna avtalet

Använd följande steg för att bjuda in en befintlig kund att granska och godkänna Microsoft-kundavtal. 

1. Skapa kundens e-postadress med den inbäddade URL:en som uppmanar kunden att godkänna Microsoft-kundavtal.

2. Kunden får inbjudan via e-post och klickar på [URL:en](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Kunden anger sina autentiseringsuppgifter i Microsoft 365 Admin Center.

4. Kunden kontrollerar rutan för att godkänna Microsoft-kundavtal. 

5. Inom samma URL kan kunden se den konsoliderade listan över olika partner som de arbetar med. De kan välja en partner för att se information.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Kunden.":::

>[!NOTE]
>I vissa fall kanske kunderna inte kan godkänna Microsoft-kundavtal. Mer information om dessa situationer finns i Två scenarier där du behöver attesta för din kunds räkning nedan.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Två scenarier där du behöver attesta för din kunds räkning

Det finns två scenarier där kunder kanske inte kan godkänna Microsoft-kundavtal i Microsoft 365 Admin Center.

**Scenario 1:** En befintlig kund har köpt något av följande via en befintlig partnerrelation: erbjudanden, programvaru- eller programvaruprenumerationer, reserverade instanser eller Azure-plan. Kunden försöker nu göra ett nytt köp (exklusive automatisk förnyelse). När kunden klickar på URL:en får de meddelandet "Kontakta din partner för att bekräfta att du godkänner Microsoft-kundavtal".  

**För att** lösa problemet måste du intyga för kundens räkning.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Skärmbild av Microsoft 365 Admin Center-sidan där du uppmanas att kontakta din partner för att bekräfta godkännandet av Microsoft-kundavtal.":::

**Scenario 2:** En befintlig kund har köpt något av följande erbjudanden, programvaru- och programvaruprenumerationer, reserverade instanser och Azure-plan. Kunden försöker nu göra ett nytt köp med en ny partner.

När kunden klickar på URL:en till Microsoft 365 Admin Center för att godkänna den nya partnerrelationen och avtalet får kunden meddelandet "Kontakta din partner för att bekräfta att du godkänner Microsoft-kundavtal".  

**För att** lösa problemet måste du intyga för kundens räkning.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Bekräfta att en kund har accepterat avtalet

Om du försöker skapa en ny order för en befintlig kund som du inte har bekräftat tidigare får du en uppmaning om att slutföra bekräftelsen. Gör detta på följande sätt.

1. Ange **förnamn,** **efternamn,** **e-postadress** och **Telefon (valfritt)** för den användare som godkände avtalet.

2. Under **Avtalets godkännandedatum** anger du lämpligt datum. Du kan inte ange detta till ett framtida datum.

3. Välj **Spara och fortsätt**. 

## <a name="next-steps"></a>Nästa steg

- [Verifiera eller uppdatera företagets profilinformation](update-your-partner-profile.md)
- [Microsoft-kundavtal (efter region, språk)](Agreements.md)
