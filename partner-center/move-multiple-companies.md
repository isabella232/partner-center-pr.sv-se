---
title: Migrera företag från PMC till Partnercenter
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vad du behöver veta när du migrerar flera företag från Partner Membership Center (PMC) till Partnercenter och konsoliderar dem till ett partner globalt konto.
author: parthpandyaMSFT
ms.author: ParthP
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2c9973bf82957cd017abfc59c25b0c17173cb3f8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151601"
---
# <a name="moving-multiple-companies-to-partner-center-from-partner-membership-center-pmc"></a>Flytta flera företag till Partnercenter från Partner Membership Center (PMC)

**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Administratörsagent | Försäljningsagent

När du flyttar ditt företagskonto från PMC till Partnercenter kan du behöva flytta flera konton. I Partnercenter konsolideras dessa konton till ett globalt konto (PGA). Det första kontot du flyttar betraktas som partnerns globala konto och alla efterföljande konton konsolideras till det första kontot som platser. Starta flytten med PMC-kontot för företagets huvudkontor. Mer information finns i [Guide to migrating from PMC to Partner Center](guide-to-migration.md) (Guide för att migrera från PMC till Partnercenter) eller titta på den här korta videon Om konton för flera platser på ett enkelt [sätt.](https://vimeo.com/290335248)

## <a name="move-your-additional-accounts-into-partner-center"></a>Flytta dina ytterligare konton till Partnercenter

Eftersom du redan har flyttat ett företagskonto till Partnercenter kommer vi att meddela dig vilket konto som redan finns i Partnercenter när du loggar in.

Om du upptäcker att fel företagskonto har angetts som juridisk verksamhet när du har migrerat kan du ändra den benämningen.

1. Gå till din **partnerprofil.**

2. Kontrollera att den plats som du vill utse som Juridisk verksamhet finns i listan över platser. Om den inte är det lägger du till den.

3. Välj **Uppdatera juridisk företagsprofil.**

4. Välj företag och region och spara den.

:::image type="content" source="images/migration/accountwithus.png" alt-text="Befintligt konto":::

## <a name="your-company-has-an-account-in-partner-center"></a>Ditt företag har ett konto i Partnercenter

Du ser ditt befintliga konto och en anteckning som talar om att din företagsinformation (det konto som du för närvarande loggar in med) kommer att konsolideras till det här kontot.

:::image type="content" source="images/migration/existingaccount2.png" alt-text="Konto i Partnercenter":::

Den här skärmen visar information om det befintliga kontot (namn och adress) som redan har skapats i Partnercenter tillsammans med information om den primära kontakten.

Välj **Fortsätt**.

## <a name="what-happens-during-consolidation-of-accounts"></a>Vad händer vid konsolidering av konton

- Du kan inte ändra någon information på den här skärmen.

- Kontot i PMC (som du flyttar) konsolideras till det befintliga kontot

- Ditt HQ och alla platser i PMC kommer att flyttas till det befintliga Partner Center-kontot som platser

- När konsolideringen är klar visas all din kontoinformation som platser i det befintliga Partnercenter-kontot

- Alla MPN-ID:er bevaras under den här konsolideringen

- Alla befintliga kompetenser (Guld/Silver), inköp (MAPS/Guld/Silver) och tillhörande förmåner bevaras under konsolideringen

- Du (användaren som loggade in med e-post-ID:t för arbetet) läggs automatiskt till som MPN-administratör och kontoadministratör för det befintliga Partnercenter-kontot så att du kan administrera kontot efter behov

## <a name="review-your-company-information"></a>Granska företagsinformation

Kontrollera informationen om ditt företag och redigera om det behövs.  Den här informationen används för att migrera ditt konto till Partnercenter, så se till att informationen är korrekt.

Informationen baseras på informationen i PMC och kommer att verifieras för att säkerställa att företaget är legitimt.


:::image type="content" source="images/migration/review.png" alt-text="Granska information":::

Om det konto som du flyttar finns i samma land eller region som det befintliga kontot kan du bestämma om du vill använda den adressen eller lägga till en annan. Om du väljer att använda en annan adress verifieras den adressen. Om du vill använda samma adress används den befintliga adressen och den primära kontakten.

När du har verifierat/redigerat informationen på den här skärmen väljer **du Skicka** så konsolideras dina konton.

## <a name="partner-profile"></a>Partnerprofil

När du visar din profil visas informationen för ditt juridiska företag (i PMC var det här huvudkontoret) och informationen för alla ytterligare platser.

## <a name="next-steps"></a>Nästa steg

- [Flytta från PMC till Partnercenter](move-pmc-pc-map.md)
- [Skapa användarkonton](create-user-accounts-and-set-permissions.md)
- [Tilldela användarroller och behörigheter](permissions-overview.md)
- [Hantera dina medlemskapsprogram](renew-mpn-offers.md)
- [Skapa företagets företagsprofil](create-a-marketing-profile.md)
- [Ansluta till kunder via hänvisningar](manage-leads.md)
