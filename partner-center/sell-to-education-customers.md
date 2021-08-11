---
title: Så här säljer du erbjudanden till utbildningskunder
description: Lär dig hur du skapar en utbildningskund och säljer erbjudanden till dem i Partnercenter. Innehåller bekräftelse av verifieringsstatus för utbildningskunden.
ms.topic: how-to
ms.date: 12/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: alikhaki
ms.author: alikhaki
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c0a88830796efa63cc6f9e2c0005b0974df22032dc877830b002527bced3a426
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115694353"
---
# <a name="how-to-sell-offers-to-education-customers-and-how-to-create-an-education-customer-in-partner-center"></a>Så här säljer du erbjudanden till utbildningskunder och hur du skapar en utbildningskund i Partnercenter

**Lämpliga roller:** Globala | Administratörsagent | Försäljningsagent

## <a name="create-an-education-customer"></a>Skapa en utbildningskund

Den här artikeln beskriver hur du skapar en utbildningskund i Partnercenter och säljer utbildningsprodukter till dem. Den beskriver också hur du visar verifieringsstatusen och skickar verifieringsbegäran igen om det behövs. Utbildningserbjudanden är för **närvarande endast tillgängliga för licensbaserade tjänster** som Microsoft 365, Dynamics, Intune osv. Den är inte tillgänglig för andra typer (programvaruprenumerationer, permanent programvara eller Azure-produkter).

> [!IMPORTANT]
> Microsoft verifierar varje nyskapad utbildningskundklientorganisation för att säkerställa att de är kvalificerade för utbildningserbjudanden.  Se till att du anger den information som krävs så korrekt och fullständigt som möjligt för att förhindra fördröjningar i verifieringsprocessen.

1. Logga in på Partner Center.

2. Välj **Kunder** och välj sedan **Lägg till en kund.** Välj **Utbildning** från **listrutan Specialkvalifikationer.**  Fyll i resten av kontoinformationen efter behov.  Viktiga fält som hjälper verifieringsprocessen är:

   - **Företagsnamn:** ANGE NAMN PÅ JURIDISK PERSON – Krävs för verifiering
   - **Land/region och adressrader:** Ange FULLSTÄNDIG ENTITETSADRESS – krävs för verifiering
   - **E-postadress:** Ange den entitetsägda e-postadressen – inte en kostnadsfri eller on.microsoft.com -e-postadress – som krävs för verifiering
   - **Kundkontaktinformation:** den här informationen används som en del av verifieringsprocessen
   - **Primärt domännamn:** Används för att skapa kundens konto och e-postadresser.  Välj ett namn som liknar företagets namn utan blanksteg eller specialtecken.  Det här namnet kan inte ändras senare.

3. När du är klar väljer du **Granska**.

   :::image type="content" source="images/eduaccountinfo.png" alt-text="Education-kundkonto.":::

4. När du har **bekräftat** Granska får du en **InReview-status** om den information som skickats är giltig. 

    :::image type="content" source="images/edu/create-review.png" alt-text="Education-kundkonto under granskning."lightbox="images/edu/create-review-expanded.png":::

### <a name="confirm-your-education-customers-verification-status"></a>Bekräfta utbildningskundens verifieringsstatus

På kundens kontosida **kan du** se **Specialkvalificeringsstatus**.
Statusexempel:

- Om kunden har klarat verifieringen: Utbildning

   :::image type="content" source="images/edupassedvetting.png" alt-text="Utbildningsverifieringen lyckades.":::

- Om kunden inte har godkänt verifieringen: Inte en utbildningskund

   :::image type="content" source="images/edu/fail-reason.png" alt-text="Utbildningsverifiering misslyckades." lightbox="images/edu/fail-reason-expanded.png":::

- Om kunden inte har taggats som Education-kund: Ingen

   :::image type="content" source="images/edu/account-one.png" alt-text="education-kunden märks inte som sådan." lightbox="images/edu/account-one-expanded.png":::

- Om kunden är under granskning som Education-kund: Granskas

    :::image type="content" source="images/edu/in-review.png" alt-text="utbildningskunden är under granskning." lightbox="images/edu/in-review-expanded.png":::

## <a name="correct-the-customer-account-info-and-resubmit-for-verification"></a>Korrigera kundkontoinformationen och skicka om för verifiering

Om kunden misslyckas med den första verifieringen kan du korrigera informationen och skicka den igen.

### <a name="correct-the-customer-account-information"></a>Rätta till informationen om kundkontot

Du måste ha behörighet som global administratör för att kunna uppdatera kundens information. Du uppdaterar informationen på Office 365 portalen eftersom dessa data inte kan uppdateras från Partnercenter-portalen.

1. På sidan **Konto** visas information om att kundkvalifikationen betraktas som "Inte utbildningskund".

2. Uppdatera webbläsaren för att återställa sidan. Det kommer att finnas **en uppdateringsknapp** **och Specialkvalifikationsstatus** har angetts till **Ingen.**

3. Välj **Uppdatera**. På sidan **Service Management** väljer du **Office 365**.

4. Du omdirigeras till Office 365 administrationscenter på en ny flik i webbläsaren. Du kan uppmanas att logga in med dina autentiseringsuppgifter.

5. Välj **inställningar**.

6. Välj **fliken Organisationsprofil** överst på skärmen och sedan **Organisationsinformation.** Nu kan du uppdatera kundinformationen.

7. Välj **Spara** ändringar längst ned i sidofältet.  

### <a name="resubmit-for-verification"></a>Skicka om för verifiering

1. Gå till fliken i Partnercenter och till **kundkontosidan.** Uppdatera webbläsaren och kontrollera att företagssidan har uppdaterats till den nya informationen. Välj **knappen Uppdatera** för att begära omverifiering av utbildning.

2. Om den uppdaterade kundinformationen är berättigad till Education-erbjudanden, kommer du att se **specialkvalifikationerna** uppdaterade till **Education**. Om du fortfarande ser **Inte utbildningskund kontaktar** du supporten för manuell verifiering.

## <a name="next-steps"></a>Nästa steg

- [Sälja till specialiserade branscher](get-special-pricing-for-offers.md)

- [Lägga till en ny kund](add-a-new-customer.md)

- [Sälja Minecraft: Education Edition-prenumerationer till utbildningskunder](minecraft-subscriptions.md)
