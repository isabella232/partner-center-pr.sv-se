---
title: Flytta från PMC till Partnercenter
ms.topic: article
ms.date: 05/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Förstå skillnaderna mellan PMC och Partnercenter vad gäller förnyelser, kontostruktur, inloggning, användarroller, kompetenser med mera.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 1729c5b6668a67e35a17c74998888324ce102c09
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146246"
---
# <a name="moving-from-partner-membership-center-pmc-to-partner-center"></a>Flytta från Partner Membership Center (PMC) till Partnercenter

**Lämpliga roller:** Global administratör

Vi gör det enklare för dig att göra affärer med oss genom att introducera en enda webbplats (Partnercenter) som fungerar som en central utgångspunkt. Allt du gjorde i Partner Membership Center (PMC) kan utföras från instrumentpanelen i Partnercenter. 

Du kan också åstadkomma mycket mer utan att lämna den enda webbplatsen. En del terminologi och funktioner kan dock se annorlunda ut. Om du vill lära dig var du utför vissa uppgifter och vilka funktioner som är tillgängliga kan du ta en rundtur på instrumentpanelen.

I den här tabellen visas några av skillnaderna mellan PMC och Partnercenter.

## <a name="renewing-your-microsoft-partner-network--membership"></a>Förnya ditt Microsoft Partner Network medlemskap

|**Pmc**   |**Partnercenter**|
|----------------------|:-----------------------------|
|Förnyelser startade 90 före årsdagen och måste ha slutförts på årsdagen| Partner kan förnya från och med dagen efter årsdagen och upp till 30 dagar efter årsdagen.|

## <a name="account-structure"></a>Kontostruktur

|**Pmc**   |**Partnercenter**|
|----------------------|:-----------------------------|
|Huvudkontor plus platser – var och en utvärderas separat. Utvärderingen av kompetenser gjordes på lokal nivå|Ett globalt företag, ditt partner-globala konto (PGA), inklusive platser, utvärderas som en helhet; prestanda- och kompetensdata aggregerade på PGA-nivå; innehåller flera profilvyer för program som partnerprofil och företagsprofil för hänvisningar och marknadsföring. Mer information finns i [Kontostrukturen i Partnercenter.](account-structure.md)|

## <a name="sign-in"></a>Logga in

|**Pmc**   |**Partnercenter**|
|----------------------|:-----------------------------|
|Kan använda din Microsoft-konto (MSA) eller personliga kontoautentiseringsuppgifter joe@outlook.com|Du måste använda autentiseringsuppgifterna för ditt arbetskonto (till exempel joe@joescompany.com ). Mer information finns i [Ditt företags arbetskonto och Partnercenter.](azure-active-directory-tenants-and-partner-center.md)|

## <a name="user-roles"></a>Användarroller

|**Pmc**   |**Partnercenter**|
|----------------------|:-----------------------------|
|Många roller i PMC används inte i Partnercenter|Den administratör som flyttar till Partnercenter tilldelas automatiskt rollerna MPN-administratör, kontoadministratör och referensadministratör. De kan sedan tilldela andra användare användarroller.|
|Användare hanterades på platsnivå|Användare hanteras på företagsnivå (PGA) i stället för på platsnivå. Undantaget är incitamentsadministratören, som fungerar på platsnivå.|
|   |Partnercenter har två breda uppsättningar roller: de roller som administrerar Azure AD-klientorganisationen och de roller som administrerar företagets verksamhet. Organisera rollerna på det sätt som är logiskt för ditt företag. En person kan göra allt eller så kan många personer tilldelas separata roller och behörigheter. Mer information finns i Tilldela [användarroller och behörigheter](permissions-overview.md). 

## <a name="how-competencies-and-benefits-are-accounted-for"></a>Så redovisas kompetenser och förmåner

|**Pmc**   |**Partnercenter**|
|----------------------|:-----------------------------|
|Påförs per plats och administreras per plats|Förmånerna gäller för hela företaget, inklusive administration av förmåner, men du kan hantera förmånerna på det sätt som bäst passar ditt företag |
|Kan ha ytterligare fördelar med verktygspaket (AKS) tills de togs ur bruk i oktober 2018.|Inga ABTK:er; en MAPS per företag; en silverkompetens per företag; en guldkompetens per företag|
||Så länge du inte redan har MAPS kan du köpa det. MAPS-ägarskapet är inte kopplat till kompetenser.  
|Du fick åtkomst till fördelarna i Partner Digital Download (PDD) |Alla fördelar nås i Partnercenter|
|Kompetenser och fördelar sprids och delas upp på flera platser|Dina kompetenser och förmåner från alla dina platser konsolideras på företagsnivå (PGA) och bevaras fram till årsdagen. Då måste du köpa eller förnya på företagsnivå. Prestanda, färdigheter och kompetenser sammanställs globalt|
|Software Assurance anspråk görs i verktyget Validering och inlösning av validering och inlösning (VVR)|Nu kan du komma åt och hantera Software Assurance TRÄNINGSutbildning (SATV) och/eller Distribuerade planeringstjänster (DPS) i Partnercenter.  Det äldre VVR-verktyget inaktiveras den 1 oktober 2019.  |

## <a name="associating-mcp-ids-to-partner-center"></a>Koppla MCP-ID:er till Partnercenter

|**Pmc**   |**Partnercenter**   |
|-------------------------|:-------------------|
|Du kan associera samma MCP-ID med flera företag.| Endast ett MCP-ID kan associeras med ett enda Partnercenter-konto. Du måste göra associationen manuellt. Från instrumentpanelen i Partnercenter väljer **du ikonen** Ditt konto i det högra hörnet på instrumentpanelen och väljer **sedan Min profil**. Under **Din utbildning** kommer du att kunna associera ditt Microsoft Learning konto och även ansluta din Microsoft-konto till Partner University.

## <a name="visual-studio-benefits-and-msa"></a>Visual Studio fördelar och MSA

|**Pmc**   |**Partnercenter**   |
|-----------------|:-----------------|
|Allokering av Visual Studio till MSA|Visual Studio fördelar som allokeras till MSA:er kommer att respekteras och behållas.|
||MSA-allokeringar av Visual Studio bevaras efter förnyelse i Partnercenter.|
||I Partnercenter kan en partner lägga till arbetskonton och gästanvändarkonton som är MSA från samma klientorganisation där partnern är MPN-administratör i Azure AD-klientorganisationen. Om partnern är global administratör i flera Azure AD-klienter och alla dessa klienter är associerade med samma Partnercenter-konto kan partnern lägga till användare över alla dessa klienter i Visual Studio-förmånerna och Användningsbaserade allokeringar för Azure. Även om gästanvändare kan tilldelas användningsbaserade prenumerationer på Visual Studio av MPN-administratören eller global administratör, kan gästanvändare inte logga in på PartnerCenter med hjälp av deras MSA. Gästanvändare kan dock logga in på Azure och Visual Studio validera och använda sina tilldelade förmåner. |

## <a name="programs-now-located-and-managed-in-partner-center"></a>Program som nu finns och hanteras i Partnercenter 

|**Pmc**   |**Partnercenter**|
|----------------------|:-----------------------------|
|Pdd  |Fördelar|
|CHIP, ICP, PIE | Incitament|
||Referenser|
|Partnerinsikter| Analys|
|Validerings- och inlösningsverktyg| Validerings- och inlösningsverktyg|
|           |Molnlösningsleverantör program|

Visual Studio fördelar som allokeras till MSA:er kommer att respekteras och behållas. De kommer också att bevaras efter förnyelsen i Partnercenter. Men om du tar bort en MSA-allokering när den har migrerats i Partnercenter kan den inte läggas till i Partnercenter igen.

I Partnercenter kan en partner lägga till arbetskonton och gästanvändarkonton, som är MSA, från samma klientorganisation där partnern är MPN-administratör i Azure AD-klienten. Om partnern är global administratör i flera Azure AD-klienter och alla dessa klienter är associerade med samma Partnercenter-konto kan partnern lägga till användare över alla dessa klienter i Visual Studio-förmånerna och Användningsbaserade allokeringar för Azure.

Även om gästanvändare kan tilldelas användningsbaserade prenumerationer på Visual Studio av MPN-administratören eller global administratör, kan gästanvändare inte logga in på PartnerCenter med hjälp av deras MSA. Gästanvändare kan dock logga in på Azure och Visual Studio validera och använda sina tilldelade förmåner.
