---
title: Flytta från PMC till Partnercenter
ms.topic: article
ms.date: 05/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Förstå skillnaderna mellan PMC-och partner Center vad gäller förnyelser, konto struktur, inloggning, användar roller, kompetenser och mycket annat.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: dae147c45aca27657f1e88b6943279f9771313d6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/01/2021
ms.locfileid: "106133003"
---
# <a name="moving-from-partner-membership-center-pmc-to-partner-center"></a>Flytta från partner medlemskaps Center (PMC) till Partner Center

**Lämpliga roller**

- Global administratör

Vi gör det enklare för dig att göra affärer med oss genom att introducera en enda webbplats (partner Center) som fungerar som en central punkt i ärendet. Du hittar allt du gjorde i partner Membership Center (PMC) kan utföras från din instrument panel i Partner Center. 

Du kan också göra mycket mer utan att lämna en webbplats. Vissa terminologier och funktioner kan se annorlunda ut. Om du vill veta var du kan göra vissa uppgifter och vilka funktioner som är tillgängliga, bör du ta plats visningen av din instrument panel.

I den här tabellen presenteras några av skillnaderna mellan PMC-och partner Center.

## <a name="renewing-your-microsoft-partner-network--membership"></a>Förnyar ditt Microsoft Partner Network medlemskap

|**PMC**   |**Partnercenter**|
|----------------------|:-----------------------------|
|Förnyelser har startat 90 före årsdag och måste ha slutförts senast dag| Partner kan förnya start dagen efter årsdagen och upp till 30 dagar efter årsdagen.|

## <a name="account-structure"></a>Konto struktur

|**PMC**   |**Partnercenter**|
|----------------------|:-----------------------------|
|Huvud kontor plus platser – varje utvärderas separat. Utvärdering av kompetenser gjordes på lokal nivå|Ett globalt företag, ditt globalt konto för partner (PGA), inklusive platser, utvärderas som helhet. prestanda-och kunskaps data som sammanställs på PGA nivå. innehåller flera profilmappar för program som partner profil och affärs profil för referenser och marknadsföring. mer information finns [i konto strukturen i Partner Center](account-structure.md).|

## <a name="sign-in"></a>Logga in

|**PMC**   |**Partnercenter**|
|----------------------|:-----------------------------|
|Kan använda dina Microsoft-konto (MSA) eller personliga konto uppgifter joe@outlook.com|Du måste använda dina autentiseringsuppgifter för ditt arbets konto (till exempel joe@joescompany.com ). Mer information finns [i företagets arbets konto och partner Center](azure-active-directory-tenants-and-partner-center.md).|

## <a name="user-roles"></a>Användarroller

|**PMC**   |**Partnercenter**|
|----------------------|:-----------------------------|
|Många roller i PMC används inte i Partner Center|Administratören som utför flytten till Partner Center tilldelas automatiskt administratörs rollerna MPN admin, Account admin och referral. De kan sedan tilldela andra användare till användar roller.|
|Användare hanterades på plats nivå|Användare hanteras på företags nivå (PGA) i stället för på plats nivån. Undantaget är stimulans administratören, som fungerar på plats nivå.|
|   |Partner Center har två breda uppsättningar roller: de roller som administrerar Azure AD-klienten och de roller som administrerar företagets verksamhet. Organisera rollerna på det sätt som passar ditt företag. En person kan göra allt eller många personer som kan tilldelas separata roller och behörigheter. Mer information finns i [Tilldela användar roller och behörigheter](permissions-overview.md). 

## <a name="how-competencies-and-benefits-are-accounted-for"></a>Hur kompetenser och förmåner redovisas

|**PMC**   |**Partnercenter**|
|----------------------|:-----------------------------|
|Periodiseras per plats och administreras per plats|Fördelarna är per hela företag, inklusive förmåns administration, men du kan hantera fördelarna på det sätt som bäst passar ditt företag |
|Det kan finnas ytterligare verktyg för Benefits Tool (ABTKs) tills de har dragits tillbaka i oktober 2018.|Ingen ABTKs; ett MAPS per företag; en silver kompetens per företag en guld-kompetens per företag|
||Så länge du inte redan har MAPS kan du köpa den. MAPS-ägarskap är inte knutna till kompetenser.  
|Förmåner har öppnats på partner Digital Download (PDD) |Alla förmåner nås i Partner Center|
|Kompetenser och fördelar sprids och delas upp på flera platser|Dina kunskaper och förmåner från alla dina platser samlas på företagets (PGA) nivå och kommer att behållas tills din jubileums dag. Vid detta tillfälle måste du köpa eller förnya på företags nivå. Prestanda, kunskaper och kompetenser samlas globalt|
|Anspråk för Software Assurance-verifikationer görs i VVR-verktyget (verifikations verifiering och inlösen)|Nu kan du komma åt och hantera Software Assurance Training-kuponger (SATV) och/eller distribuerade planerings tjänster (DPS) i Partner Center.  Det äldre VVR-verktyget tas ur drift den 1 oktober 2019.  |

## <a name="associating-mcp-ids-to-partner-center"></a>Associera MCP-ID: n till Partner Center

|**PMC**   |**Partnercenter**   |
|-------------------------|:-------------------|
|Du kan associera samma MCP-ID till flera företag.| Endast ett MCP-ID kan associeras med ett enda partner Center-konto. Du måste skapa kopplingen manuellt. Från instrument panelen för partner Center väljer du **ditt konto** -ikonen i det högra hörnet av instrument panelen och väljer **min profil**. Under **din utbildning** kommer du att kunna associera ditt Microsoft Learning-konto och ansluta din Microsoft-konto till partner University.

## <a name="visual-studio-benefits-and-msa"></a>Visual Studio-förmåner och MSA

|**PMC**   |**Partnercenter**   |
|-----------------|:-----------------|
|Allokering av Visual Studio-förmåner till MSA|Visual Studio-förmåner som tilldelas till MSA: er kommer att behållas och behållas.|
||MSA allokeringar av Visual Studio kommer att bevaras efter förnyelse i Partner Center.|
||I Partner Center kan en partner lägga till arbets konton och gäst användar konton som är MSA från samma klient organisation där partnern är MPN-administratör i Azure AD-klienten. Om partnern är global administratör i flera Azure AD-klienter och alla dessa klienter är kopplade till samma Partner Center-konto, tillåts partnern att lägga till användare över alla dessa klienter i Visual Studio-förmånerna och Azure Usage-baserade allokeringar. Gäst användare kan tilldelas användnings prenumerationer av Visual Studio av MPN-administratören eller den globala administratören, men gäst användare kan inte logga in på Partner Center med hjälp av deras MSA. Gäst användare kan dock logga in på Azure och Visual Studio för att validera och använda sina tilldelade förmåner. |

## <a name="programs-now-located-and-managed-in-partner-center"></a>Program som nu finns och hanteras i Partner Center 

|**PMC**   |**Partnercenter**|
|----------------------|:-----------------------------|
|PDD  |Fördelar|
|CHIP, ICP, CIRKEL | Incitament|
||Referenser|
|Partner Insights| Analys|
|Verktyg för validering och inlösen av verifikationer| Verktyg för validering och inlösen av verifikationer|
|           |Cloud Solution Provider-program|

Visual Studio-förmåner som tilldelas till MSA: er kommer att behållas och behållas. De kommer också att bevaras efter förnyelse i Partner Center. Men om du tar bort en MSA-allokering när du har migrerat i Partner Center kan du inte lägga till den i Partner Center igen.

I Partner Center kan en partner lägga till arbets konton och gäst användar konton, som är MSA, från samma klient organisation där partnern är MPN-administratör i Azure AD-klienten. Om partnern är global administratör i flera Azure AD-klienter och alla dessa klienter är kopplade till samma Partner Center-konto, tillåts partnern att lägga till användare över alla dessa klienter i Visual Studio-förmånerna och Azure Usage-baserade allokeringar.

Gäst användare kan tilldelas användnings prenumerationer av Visual Studio av MPN-administratören eller den globala administratören, men gäst användare kan inte logga in på Partner Center med hjälp av deras MSA. Gäst användare kan dock logga in på Azure och Visual Studio för att validera och använda sina tilldelade förmåner.
