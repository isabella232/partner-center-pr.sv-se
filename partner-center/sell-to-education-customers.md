---
title: Så här säljer du erbjudanden till utbildningskunder
description: Lär dig hur du skapar en utbildningskund och säljer erbjudanden till dem i Partnercenter. Omfattar bekräftelse av verifieringsstatus för utbildningskunden.
ms.topic: how-to
ms.date: 12/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: alikhaki
ms.author: alikhaki
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2d9924b8d361be4237c613467a1d36db29cf7d9e
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247111"
---
# <a name="how-to-sell-offers-to-education-customers-and-how-to-create-an-education-customer-in-partner-center"></a>Så här säljer du erbjudanden till utbildningskunder och hur du skapar en utbildningskund i Partnercenter

**Lämpliga roller:** Global | Administratörsagentens | Försäljningsagent

## <a name="create-an-education-customer"></a>Skapa en utbildningskund

Den här artikeln förklarar hur du skapar en utbildningskund i Partnercenter och säljer utbildningsprodukter till dem. Den beskriver också hur du visar verifieringsstatusen och skickar verifieringsbegäran igen om det behövs. Utbildningserbjudanden är för **närvarande endast tillgängliga för licensbaserade tjänster** som Microsoft 365, Dynamics, Intune osv. Den är inte tillgänglig för andra typer (programvaruprenumerationer, permanent programvara eller Azure-produkter).

> [!IMPORTANT]
> Microsoft verifierar varje nyskapad utbildningsklientorganisation för att säkerställa att de är kvalificerade för utbildningserbjudanden.  Se till att du anger den information som krävs så korrekt och fullständigt som möjligt för att förhindra fördröjningar i verifieringsprocessen.

1. Logga in på Partner Center.

2. Välj **Kunder** och välj sedan **Lägg till en kund.** Välj **Utbildning** i **listrutan Specialkvalifikationer.**  Fyll i resten av kontoinformationen efter behov.  Viktiga fält som hjälper verifieringsprocessen är:

   - **Företagsnamn:** ANGE NAMN PÅ JURIDISK PERSON – Krävs för verifiering
   - **Lands-/region- och adressrader:** Ange FULLSTÄNDIG ENTITETSADRESS – krävs för verifiering
   - **E-postadress:** Ange den entitetsägda e-postadressen – inte ett kostnadsfritt eller on.microsoft.com-e-postmeddelande – som krävs för verifiering
   - **Kundkontaktinformation:** den här informationen används som en del av verifieringsprocessen
   - **Primärt domännamn:** Används för att skapa kundens konto och e-postadresser.  Välj ett namn som liknar företagets namn utan blanksteg eller specialtecken.  Det här namnet kan inte ändras senare.

3. När du är klar väljer du **Granska**.

   :::image type="content" source="images/eduaccountinfo.png" alt-text="Education-kundkonto.":::

4. När du har **bekräftat Granska** får du **statusen InReview** om den information som skickats är giltig. 

    :::image type="content" source="images/edu/create-review.png" alt-text="Education-kundkonto som granskas."lightbox="images/edu/create-review-expanded.png":::

### <a name="confirm-your-education-customers-verification-status"></a>Bekräfta din utbildningskunds verifieringsstatus

På kundens kontosida **kan du** se **Specialkvalificeringsstatus**.
Statusexempel:

- Om kunden har klarat verifieringen: Utbildning

   :::image type="content" source="images/edupassedvetting.png" alt-text="Utbildningsverifieringen lyckades.":::

- Om kunden inte har godkänt verifieringen: Inte en utbildningskund

   :::image type="content" source="images/edu/fail-reason.png" alt-text="Utbildningsverifieringen misslyckades." lightbox="images/edu/fail-reason-expanded.png":::

- Om kunden inte har taggats som Education-kund: Ingen

   :::image type="content" source="images/edu/account-one.png" alt-text="education-kund har inte taggats som sådan." lightbox="images/edu/account-one-expanded.png":::

- Om kunden är under granskning som Education-kund: Granskas

    :::image type="content" source="images/edu/in-review.png" alt-text="education-kund är under granskning." lightbox="images/edu/in-review-expanded.png":::

## <a name="correct-the-customer-account-info-and-resubmit-for-verification"></a>Korrigera kundkontoinformationen och skicka om för verifiering

Om kunden misslyckas med den första verifieringen kan du korrigera informationen och skicka den igen.

### <a name="correct-the-customer-account-information"></a>Rätta till informationen om kundkontot

Du måste ha behörighet som global administratör för att kunna uppdatera kundens information. Du uppdaterar informationen på Office 365 portalen eftersom dessa data inte kan uppdateras från Partnercenter-portalen.

1. På sidan **Konto** visas information om att kundkvalifikationen betraktas som "Inte utbildningskund".

2. Uppdatera webbläsaren för att återställa sidan. Det kommer att finnas **en uppdateringsknapp** **och Status för specialkvalifikationer** har angetts till **Ingen.**

3. Välj **Uppdatera**. På sidan **Tjänsthantering** väljer du **Office 365**.

4. Du omdirigeras till Office 365 administrationscenter på en ny flik i webbläsaren. Du kan uppmanas att logga in med dina autentiseringsuppgifter.

5. Välj **inställningar**.

6. Välj **fliken Organisationsprofil** överst på skärmen och sedan **Organisationsinformation.** Nu kan du uppdatera kundinformationen.

7. Välj **Spara ändringar** längst ned i sidofältet.  

### <a name="resubmit-for-verification"></a>Skicka om för verifiering

1. Gå till fliken i Partnercenter och till **kundkontosidan.** Uppdatera webbläsaren och kontrollera att sidan Företag har uppdaterats till den nya informationen. Välj **knappen** Uppdatera för att begära omverifiering av utbildning.

2. Om den uppdaterade kundinformationen är berättigad till Education-erbjudanden visas specialkvalifikationerna **uppdaterade** till **Education**. Om du fortfarande ser **Inte utbildningskund kontaktar** du supporten för manuell verifiering.

## <a name="next-steps"></a>Nästa steg

- [Sälja till specialiserade branscher](get-special-pricing-for-offers.md)

- [Lägga till en ny kund](add-a-new-customer.md)

- [Sälja Minecraft: Education Edition prenumerationer till utbildningskunder](minecraft-subscriptions.md)
