---
title: Migrera företag från PMC till Partner Center
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vad du behöver veta när du migrerar flera företag från partner medlemskaps Center (PMC) till Partner Center och konsoliderar dem till ett globalt partner konto.
author: parthpandyaMSFT
ms.author: ParthP
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 459f347d960a06f78a30a398dc51b67f2fa7d27b
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531604"
---
# <a name="moving-multiple-companies-to-partner-center-from-partner-membership-center-pmc"></a>Flytta flera företag till Partner Center från partner medlemskaps Center (PMC)

**Lämpliga roller**

- Global administratör
- Användaradministratör
- Administratörs agent
- Försäljnings agent

När du flyttar ditt företagskonto från PMC till Partnercenter kan du behöva flytta flera konton. Dessa konton samlas in i ett globalt konto (PGA) i Partner Center. Det första kontot som du flyttar kommer att anses som globalt konto för partnern och alla efterföljande konton samlas in i det första kontot som platser. Starta flytten med PMC-kontot för företagets huvud kontor. Mer information finns i [Guide för att migrera från PMC till Partner Center](guide-to-migration.md) eller titta på det här korta video [kontot för flera platser](https://vimeo.com/290335248).

## <a name="move-your-additional-accounts-into-partner-center"></a>Flytta ytterligare konton till Partner Center

Eftersom du redan har flyttat ett företags konto till Partner Center, kommer vi att meddela dig vilket konto som redan finns i Partner Center när du loggar in.

Om du upptäcker att fel företags konto har angetts som juridisk verksamhet när du har migrerat, kan du ändra den beteckningen.

1. Gå till din **partner profil.**

2. Kontrol lera att den plats som du vill ange som juridisk verksamhet finns i listan över platser. Om den inte är det lägger du till den.

3. Välj **Uppdatera juridisk företags profil.**

4. Välj företag och region och spara.

:::image type="content" source="images/migration/accountwithus.png" alt-text="Befintligt konto":::

## <a name="your-company-has-an-account-in-partner-center"></a>Ditt företag har ett konto i Partner Center

Du ser ditt befintliga konto och en anteckning som visar att företagets information (det konto som du loggar in med) samlas in i det här kontot.

:::image type="content" source="images/migration/existingaccount2.png" alt-text="Befintligt konto":::

På den här skärmen visas information om det befintliga kontot (namn och adress) som redan har skapats i Partner Center tillsammans med information om den primära kontakten.

Välj **Fortsätt** .

## <a name="what-happens-during-consolidation-of-accounts"></a>Vad händer under konsolidering av konton

- Du kan inte ändra någon information på den här skärmen.

- Kontot i PMC (som du flyttar för närvarande) kommer att samlas in i det här befintliga kontot

- Din HQ och alla platser i PMC kommer att flyttas till det här befintliga partner Center-kontot som platser

- När konsolideringen är klar visas alla konto uppgifter som platser i det befintliga partner Center-kontot

- Alla MPN-ID: n bevaras under denna konsolidering

- Alla dina befintliga kompetenser (Gold/Silver), inköp (kartor/guld/silver) och tillhör ande förmåner bevaras under konsolideringen

- Du (användaren som loggade in med e-postadressen för arbetet) läggs automatiskt till som MPN-administratör och en konto administratör till det befintliga partner Center-kontot så att du kan administrera kontot efter behov

## <a name="review-your-company-information"></a>Granska företagets information

Kontrol lera informationen om ditt företag och redigera vid behov.  Informationen kommer att användas för att migrera ditt konto till Partner Center, så se till att informationen är korrekt.

Informationen baseras på informationen i PMC och kommer att kontrol leras för att säkerställa att företaget är legitimt.


:::image type="content" source="images/migration/review.png" alt-text="Befintligt konto":::

Om kontot du flyttar finns i samma land eller region som det befintliga kontot kan du välja om du vill använda adressen eller lägga till en annan. Om du väljer att använda en annan adress kommer den adressen att verifieras. Om du vill använda samma adress kommer den befintliga adressen och den primära kontakten att användas.

När du har verifierat/redigerat informationen på den här skärmen klickar du på Skicka så kommer dina konton att konsol IDE ras.

## <a name="partner-profile"></a>Partner profil

När du visar din profil visas informationen för din juridiska verksamhet (i PMC detta var huvud kontor) och information för alla ytterligare platser.

## <a name="next-steps"></a>Nästa steg

- [Flytta från PMC till Partnercenter](move-pmc-pc-map.md)
- [Skapa användar konton](create-user-accounts-and-set-permissions.md)
- [Tilldela användarroller och behörigheter](permissions-overview.md)
- [Hantera dina medlemskaps program](renew-mpn-offers.md)
- [Skapa företagets företags profil](create-a-marketing-profile.md)
- [Ansluta till kunder via hänvisningar](manage-leads.md)
