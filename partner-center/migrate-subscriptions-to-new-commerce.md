---
title: Migrera prenumerationer till ny handel
ms.topic: article
ms.date: 10/04/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig mer om nya handelsupplevelser för att migrera prenumerationer.
author: iragulati1
ms.author: iragulati
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bad50c36cd0e0523fe70115e0b39d88e0e68ab68
ms.sourcegitcommit: 462d6026287b85c9feea602af5bcdf924f3e6976
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/05/2021
ms.locfileid: "129454670"
---
# <a name="introduction-migrate-subscriptions-to-new-commerce"></a>Introduktion: Migrera prenumerationer till ny handel

**Lämpliga roller:** Administratörsagent | Försäljningsagent | Global administratör

> [!NOTE]
> Ändringarna i den nya handelsupplevelsen är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.
Partner kan migrera prenumerationer till New Commerce om prenumerationen uppfyller behörighetskriterierna och det finns en tillgänglig typ av erbjudande.

## <a name="ineligible-subscriptions"></a>Icke-liga prenumerationer ##

Alla prenumerationer är inte berättigade till migrering just nu. Följande kategorier av prenumerationer är för närvarande inte liga: 

- Inaktiva prenumerationer (inga ändringar i tjänsten sker om en prenumeration är inaktiv) 

- Utvärderingsprenumerationer (inga ekonomiska fördelar eller effekter. Förväntningen är att låta utvärderingsversioner köra kursen i Legacy) 

- Prenumerationer med kampanjer (kampanjer i NCE är oberoende av dessa kampanjer i Legacy) 

- Prenumerationer med tillägg (migrering av prenumerationer med tillägg kommer att aktiveras senare. Just nu kan vi inte stödja samtidig migrering) 

- Prenumerationer för gov-, edu- eller ideella målgrupper (mappning av kvalificerade erbjudanden från Legacy till NCE stöds inte) 

- Inaktuella eller inaktuella prenumerationer (för dessa prenumerationer kommer det inte att finnas någon like-like-erbjudande i New Commerce) 

Migreringar av ovanstående prenumerationer ligger utanför omfånget för den här funktionen just nu. Dessutom blir en enskild prenumeration migreringsenheten i stället för batchar med prenumerationer. 

## <a name="suspending-a-legacy-subscription-during-migration"></a>Pausa en äldre prenumeration under migreringen ##

En äldre prenumeration pausas bara när en lyckad sökväg till Ny handel har etablerats för prenumerationen. Den här funktionen förhindrar tjänstförlust om det finns några blockerare efter en partner som påbörjar migreringen av en prenumeration. Dessutom sker ingen dubbel fakturering för både den äldre och den nya handelsprenumerationen. När migreringen har påbörjats stoppas faktureringen för den äldre prenumerationen för att förhindra eventuell överlappning med faktureringen för NCE-prenumerationen.

## <a name="billing-term-and-frequency"></a>Faktureringsperiod och -frekvens ##

Faktureringsperioden och faktureringsfrekvensen för den migrerade prenumerationen förblir desamma som faktureringsperioden och faktureringsfrekvensen för den äldre prenumerationen. slutdatumet förblir detsamma.

## <a name="new-commerce-promotions"></a>Nya handelskampanjer ##

Prenumerationer i äldre med kampanjer är inte berättigade till migrering. Migrerade prenumerationer kan vara berättigade till introduktionskampanjer om ny handel. Kampanjerna kommer att proreras till resten av prenumerationsperioden vid tidpunkten för migreringen. 

## <a name="cancelling-subscriptions-or-decreasing-licenses"></a>Avbryta prenumerationer eller minska licenser ##

Efter migreringen finns det en 72-timmars annulleringsfönster. Under de här 72 timmarna kan partner avbryta prenumerationen eller minska licenskvantiteten i det här fönstret. När 24-timmarsmarkeringen har gått sedan migreringen slutfördes, kommer annulleringar av prenumerationen eller licenser att prorreras för en dag av användning. Efter 48-timmarsmarkeringen sedan migreringen slutfördes, kommer annulleringar av prenumerationen eller licenser att ske i två dagar efter att prenumerationen eller licenserna har avslutats. 

## <a name="migration-history"></a>Migreringshistorik ##

Via API:erna kan du komma åt information om migreringshistorik, till exempel start- och slutförandevillkor för migrering med hjälp av det nya getmigration-API:et och fältet MigrationID. På UX visas prenumerations-ID:t som den nya NCE-prenumerationen migrerades från överst på informationssidan, som du kommer åt när du klickar på prenumerationsradobjektet på kundens sida "Prenumerationer". 

## <a name="apis"></a>API:er ##

Vid migrering av liknande prenumerationer kommer det att släppas tre nya REST-API:er. Det första "CheckMigration"-API:et kontrollerar berättigandet för migrering för en prenumeration. Det andra "CreateMigration"-API:et skapar migreringen om prenumerationen är berättigad. Slutligen gör det tredje GETMigration-API:et att partner kan kontrollera migreringsstatusen. 
