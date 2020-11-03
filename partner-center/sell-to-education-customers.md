---
title: Hur du säljer erbjudanden till utbildnings kunder
description: Lär dig hur du skapar en utbildnings kund och säljer erbjudanden till dem i Partner Center. Inkluderar bekräftelse av verifierings status för din utbildnings kund.
ms.topic: how-to
ms.date: 10/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: alikhaki
ms.author: alikhaki
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5f17493a55ebd7d1ff9de0570e867cdf38e2e3fb
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532001"
---
# <a name="how-to-sell-offers-to-education-customers--how-to-create-an-education-customer-in-partner-center"></a>Hur du säljer erbjudanden till utbildnings kunder & hur man skapar en utbildnings kund i Partner Center

**Gäller för**

- Partnercenter

**Lämpliga roller**

- Global administratör
- Administratörs agent
- Försäljnings agent

## <a name="create-an-education-customer"></a>Skapa en utbildnings kund

Den här artikeln beskriver hur du skapar en utbildnings kund i Partner Center och säljer utbildnings produkter till dem. Det beskriver också hur du visar verifierings statusen och skickar om verifierings förfrågan om det behövs.

> [!IMPORTANT]
> Microsoft verifierar varje nyskapad kund klient organisation för att säkerställa att de är kvalificerade för utbildnings erbjudanden.  Se till att du anger den information som krävs så fort som möjligt för att förhindra fördröjningar i verifierings processen.

1. Logga in på Partner Center.

2. Välj **kunder** och välj sedan **Lägg till en kund** . Välj **utbildning** i list rutan **särskilda kvalifikationer** .  Fyll i resten av konto informationen efter behov.  Nyckel fält som underlättar verifierings processen:

   - **Företags namn** : Ange juridisk enhets namn – krävs för verifiering
   - **Land/region och adress rader** : Ange fullständig e-postadress för entitet – krävs för verifiering
   - **E-post adress** : ange entitetens ägda e-postadress – inte ett kostnads fritt eller on.Microsoft.com e-postmeddelande – krävs för verifiering
   - **Kund kontakt information** : den här informationen kommer att användas som en del av verifierings processen
   - **Primärt domän namn** : används för att skapa kundens konto och e-postadresser.  Välj ett namn som liknar företagets namn utan blank steg eller specialtecken.  Det här namnet kan inte ändras senare.

3. När du är klar väljer du **Granska** .

   :::image type="content" source="images/eduaccountinfo.png" alt-text="Utbildnings kund konto":::

### <a name="confirm-your-education-customers-verification-status"></a>Bekräfta din kunds verifierings status

På sidan kund **konto** , se status för **särskilda kvalifikationer** .
Status exempel:

- Om kunden lyckades verifiera: utbildning

   :::image type="content" source="images/edupassedvetting.png" alt-text="Utbildnings kund konto":::

- Om kunden inte klarade verifieringen: inte en utbildnings kund

   :::image type="content" source="images/edudidnotpassvetting.png" alt-text="Utbildnings kund konto":::

- Om kunden inte har taggats som en utbildnings kund: ingen

   :::image type="content" source="images/edunottagged.png" alt-text="Utbildnings kund konto":::

## <a name="correct-the-customer-account-info-and-resubmit-for-verification"></a>Korrigera kund konto informationen och skicka om verifieringen

Om kunden inte kan utföra den första verifieringen kan du nu korrigera informationen och skicka den igen.

### <a name="correct-the-customer-account-information"></a>Korrigera kund konto informationen

Du måste ha global administratörs behörighet för att uppdatera kundens information. Du uppdaterar informationen på Office 365-portalen eftersom det inte går att uppdatera data från Partner Center-portalen.

1. På sidan **konto** visas information om att kund kvalifikationen betraktas som "inte en utbildnings kund".

2. Uppdatera webbläsaren för att återställa sidan. Det kommer att finnas en **uppdaterings** knapp och **särskild kompetens status** är inställd på **ingen** .

3. Välj **Uppdatera** . På sidan **tjänst hantering** väljer du **Office 365** .

4. Du omdirigeras till administrations centret för Office 365 på en ny flik i webbläsaren. Du kan uppmanas att logga in med dina autentiseringsuppgifter.

5. Välj **Inställningar** .

6. Välj fliken **organisations profil** överst på skärmen och sedan **organisations information** . Nu kan du uppdatera kund informationen.

7. Välj **Spara ändringar** längst ned i marginal listen.  

### <a name="resubmit-for-verification"></a>Skicka om för verifiering

1. Gå till fliken Partner Center och på sidan kund **konto** . Uppdatera webbläsaren och kontrol lera att företags sidan har uppdaterats till den nya informationen. Välj knappen **Uppdatera** för att begära omverifiering av utbildning.

2. Om den uppdaterade kund informationen är kvalificerad för utbildnings erbjudanden kan du se de **särskilda kvalifikationerna** som har uppdaterats för **utbildning** . Kontakta supporten för manuell verifiering om du fortfarande ser att det **inte finns någon utbildnings kund** .

## <a name="next-steps"></a>Nästa steg

- [Sälj till specialiserade branscher](get-special-pricing-for-offers.md)

- [Lägg till en ny kund](add-a-new-customer.md)

- [Sälj Minecraft: utbildnings Edition-prenumerationer på utbildnings kunder](minecraft-subscriptions.md)
