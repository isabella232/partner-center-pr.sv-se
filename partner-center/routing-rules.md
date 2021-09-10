---
title: Skapa och hantera routningsregler för inkommande affärsmöjligheter
ms.topic: article
ms.date: 08/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ditt företag kan skapa regler för att bestämma hur en inkommande möjlighet till säljförsäljning från Microsofts säljare dirigeras.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: efb76953b05bfb10a18657155349e267ee84f456
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961476"
---
# <a name="create-and-manage-inbound-opportunities-routing-rules"></a>Skapa och hantera routningsregler för inkommande affärsmöjligheter

**Lämpliga roller:** Referensadministratörsroller | Referensanvändare

> [!IMPORTANT]
> **Det är valfritt att skapa routningsregler.** Det rekommenderas endast för större företag med närvaro över hela världen eller om ditt företag har en komplex MPN-hierarki där hänvisningshantering ska göras på en viss platsnivå baserat på kundmarknad och lösningar.

## <a name="introduction"></a>Introduktion

Funktionerna som beskrivs i det här dokumentet hjälper ditt företag att konfigurera regler som kan hjälpa dig att dirigera de möjligheter till säljförsäljning som Microsoft-säljare skickar till valfri MPN-plats. Som standard skickas hänvisningarna från Microsoft-säljaren till den MPN-plats som är associerad med samförsäljningslösningen som ingår i affärsmöjligheten. Routningsreglerna om de skapas hjälper ditt företag att åsidosätta standardroutning. Endast [**referensadministratörer**](permissions-overview.md#manage-referrals) med hela organisationens omfång kan skapa och redigera routningsregler. Partner med [**referensanvändarroll**](permissions-overview.md#manage-referrals) kan bara visa routningsreglerna för att förstå hur hänvisningar dirigeras inom företaget.

Reglerna tillämpas inte i efterhand. Referenser som skapats tidigare eller med en äldre konfiguration av routningsregeln uppdateras inte. Ändringar som görs i reglerna gäller omedelbart.

Det finns tre huvudsakliga pivoter för alla regler.

- **Kundmarknad** – Den marknad där kundföretaget finns

- **Lösning** – lösningar som publicerats av ditt företag antingen via OCP GTM-portalen eller den kommersiella marknadsplatsen

- **MPN-plats** – DEN MPN-plats som hänvisningen ska dirigeras till

Varje regel kan läsas som – För hänvisningar som skickas av Microsoft-säljare med lösningar från mitt företag kan du dirigera dem till den **här MPN-platsen**

> [!Note]
> Regler för inkommande routning gäller endast för möjligheter till säljförsäljning som skickas av Microsoft-säljare till ditt företag.

## <a name="navigation"></a>Navigering

Du kan skapa routningsregler på **fliken Referenser** under **sidan Kontoinställningar.** Om du vill navigera till sidan väljer du **inställningsikonen** bredvid användarikonen i det övre högra hörnet och väljer sedan fliken Referenser i det vänstra navigeringsfönstret.

## <a name="initial-setup"></a>Inledande konfiguration

**Att konfigurera routningsregler är inte obligatoriskt.** Om ditt företag bestämmer sig för att använda routningsreglerna för att dra nytta av routningslogiken kan du börja med att importera standardreglerna som referenshanteringssystemet använder för att dirigera hänvisningarna. Den aktuella logiken använder det MPN-ID som är associerat med lösningen för att dirigera alla inkommande hänvisningar från Microsoft-säljare oavsett kundens land. De är tillgängliga för din referens och **kan importeras med ett klick som** routningsregler. När importåtgärden har slutförts tillämpas reglerna för alla nya hänvisningar som skickas av Microsoft-säljare. Ditt företag kan redigera eller ta bort befintliga regler och skapa nya regler om det behövs. Endast [**referensadministratör**](permissions-overview.md#manage-referrals) med globalt omfång kan importera reglerna. Samma behörighet krävs för alla efterföljande ändringar i routningsreglerna.

> [!IMPORTANT]
> **Det finns ändringar i logiken för e-postaviseringar.** Så snart reglerna har importerats skickas inte längre  de e-postmeddelanden som tidigare skickades till lösningskontakter som laddades upp på fliken Samförsäljning på den kommersiella marknadsplatsen. **Endast [hänvisningsadministratörer](permissions-overview.md#manage-referrals)** för den MPN-plats som samförsäljningsmöjligheten skickas till meddelas.

## <a name="override-rules"></a>Åsidosätt regler

Du kan åsidosätta två typer av regler och åsidosätta ett specifikt villkor för standardregeln. I standardregeln kan du bara ändra den MPN-plats som hänvisningarna ska dirigeras till. De andra två regeltyperna som du kan åsidosätta är de med **Alla lösningar** och **Alla marknader** som villkor i reglerna.

**Åsidosätt alla marknader** – Förutsatt att du har skapat en regel som säger att för alla kundmarknadar och en viss lösning A dirigerar du hänvisningarna till MPN-platsen M1. Du kan åsidosätta den här regeln med en specifik marknad och samma lösningskombination. Exempelåsidosättning kan vara "för hänvisningar som innehåller kunder från marknaden Storbritannien och lösning A dirigerar du den till MPN-platsen M2.

**Åsidosätt alla lösningar** – Förutsatt att du har skapat en regel som säger att för alla lösningar och en viss marknad MKT1 dirigerar du hänvisningarna till MPN-platsen M1. Du kan åsidosätta en sådan regel med en specifik lösning och samma kombination av marknad. Exempelåsidosättning kan vara "för hänvisningar som innehåller kunder från marknaden MKT1 och lösning B dirigerar du den till MPN-platsen M2.

Tabellen nedan visar en sammanfattning av de typer av lösningar som du kan åsidosätta

| **Typ** | **Kan du åsidosätta ?** |
|-------|-------|
|Standardvärde| No |
|Alla marknader| Yes|
|Alla lösningar| Yes|
|En eller flera specifika lösningar och specifika marknadskombinationer| No|

> [!Note]
> Du kan ändra MPN-platsen för standardregeln även om du inte kan ändra något annat i regeln.

## <a name="rules-evaluation"></a>Utvärdering av regler

Om ditt företag har flera regler som kan tillämpas för ett scenario, under de utvärderingskriterier som används.

- Den första kontrollen är för en regel med den specifika lösningen och marknadskombinationen, som är i den inkommande affärsmöjligheten. En direkt matchning till en sådan regel har företräde framför alla andra regler.
- Om den första kontrollen misslyckas kontrollerar vi om det finns några regler som innehåller den lösning som nämns i hänvisningen med ett marknadsvillkor som angetts som alla marknader.
- Om den andra kontrollen misslyckas kontrollerar vi om det finns några regler där alla lösningar nämns som lösningskriterier för en specifik marknad.
- Om den tredje kontrollen också misslyckas använder vi standardregeln.

> [!Note]
> Du kan inte skapa en regel som står i konflikt med andra regler på en specifik plats- och lösningsnivå. Användargränssnittet orsakar ett fel med namnet på regeln som står i konflikt med konfigurationen om du försöker skapa en regel som står i konflikt.

## <a name="example"></a>Exempel

Regler för inkommande routning förklaras med hjälp av routningsregler som skapats för Contoso Corporation. Innan vi förstår hur reglerna kommer att tillämpas ska vi förstå MPN-hierarkin och användaruppsättningen på Contoso Corporation.

#### <a name="mpn-hierarchy-of-contoso-corporation"></a>MPN-hierarki för Contoso Corporation

| **MPN-ID** | **Typ** | **Adress** |
|-------|-------|-------|
|999999| Global| One Contoso way, **Redmond, USA of America**|
|555555| Location| One Contoso way, **London, Storbritannien**|
|666666| Location| One Contoso way, **Singapore, Singapore**|
|777777| Location| One Contoso way, **Samtidige, Indien**|

#### <a name="sellers-from-contoso-corporation"></a>Säljare från Contoso Corporation

Nedan visas säljarna med sina respektive hänvisningsroller och omfång på Contoso Corporation.

| **Namn** | **Role** | **Omfång** |
|-------|-------|-------|
|Seller One|Referensadministratör|Hela organisationen|
|Seller Two|Referensadministratör|Bengaluru|
|Seller Three|Referensanvändare|London|
|Seller Four|Referensanvändare|Singapore|

#### <a name="inbound-routing-rules-for-contoso-corporation"></a>Regler för inkommande routning för Contoso Corporation

Anta att nedanstående uppsättning regler har skapats av Seller 1 för Contoso Corporation. Endast **Seller One** kan skapa dessa regler eftersom [referensadministratör i](permissions-overview.md#manage-referrals) hela organisationens omfång krävs för att skapa och redigera regler.

| **Marknader** | **Lösningar** | **MPN-plats** | **Namn på routningsregel** |
|-------|-------|-------|-------|
|Alla marknader|Alla lösningar|Redmond|Standardvärde|
|Storbritannien|Alla lösningar|London|Storbritannien – alla lösningar|
|Alla marknader|Sol-ABC|Singapore|Sol-ABC – alla marknader|
|Indien|Sol-PQR|Bengaluru|India-Sol-PQR|

#### <a name="summary-of-routing-for-various-scenarios-based-on-the-rules-for-contoso-corporation"></a>Sammanfattning av routning för olika scenarier baserat på reglerna för Contoso Corporation

| **Nej** | **Scenario** | **Kundmarknad** | **Lösningar som ingår** |**Routningsregel tillämpad** |**MPN-tilldelning** |**Åtkomst till referenser** |
|-----|----------|-------|-------|-------|-------|-----------|
| 1|Ingen specifik lösning och regelmatchning på marknaden|Storbritannien|SOL-PQR|Global|999999| Seller One, Seller Two, Seller Three (om de läggs till i teamet), Seller Four(om de läggs till i teamet)|
| 2|Alla lösningar och en specifik regelmatchning för marknaden|Storbritannien|SOL-PQR|Storbritannien – alla lösningar|555555| Seller One, Seller Three (om det läggs till i teamet) |
| 3|Specifik lösning och regelmatchning för alla marknader|Nigeria|SOL-ABC|SOL-ABC – alla marknader|666666| Seller One, Seller Four (om de läggs till i teamet) |
| 4|Specifik lösning och regelmatchning för marknaden|Indien|SOL-PQR|India-Sol-PQR|777777| Seller One, Seller Two|
| 5|Inkommande hänvisning med en lösning som inte ägs av ditt företag|USA för USA|SOL-XYZ|Global|999999| Seller One, Seller Two, Seller Three (om de läggs till i teamet), Seller Four(om de läggs till i teamet)|

## <a name="next-steps"></a>Nästa steg

- [Hantera möjligheter till säljförsäljning](manage-co-sell-opportunities.md)

- [Hämta anslutningsappen för säljförsäljning för Dynamics 365 CRM](connector-dynamics.md)

- [Hämta anslutningsappen för säljförsäljning för Salesforce CRM](connector-salesforce.md)
