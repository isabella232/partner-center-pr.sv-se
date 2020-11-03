---
title: Felsöka samsäljande referral-kopplingar
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig svar på vanliga frågor om att använda samförsäljnings anslutningar. Läs vanliga frågor och svar om hur du felsöker samförsäljnings anslutningar.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/14/2020
ms.locfileid: "92531889"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Felsöka samsäljande referral-kopplingar

**Gäller för:**

- Partnercenter
- Dynamics 365 CRM
- Salesforce CRM

**Lämpliga roller**

- Referens administratör
- System administratör eller systemanpassare på CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Frågor och svar om krav

1. Kan du använda en lösning för att använda en utvärderings version av referral Connector för din miljö?

Om du är i test-/Staging-miljön kan du välja en utvärderings lösning. Den betalda versionen av kopplingarna är tillgänglig i AppSource till USA $15/månad. Med den betalda anslutningen kommer du att få 10 000 API-anrop per dag. Kopplingarna är omslutningar ovanpå partner Centers hänvisnings-API: er. När kopplings lösningarna körs för att **skapa** eller **Uppdatera** en händelse för affärs möjligheter i antingen Partner Center eller på CRM-sidan, görs ett API-anrop.

2. Vilken roll behöver du för att skapa avsnitt i CRM-miljön?

Användare som är system administratörer eller systemanpassare kan tillämpa ändringar för alla. Alla App-användare kan dock anpassa systemet och till och med dela vissa av deras anpassningar med andra. 

3. Behöver partner leverantörer särskilda roller för att arbeta med partner Center?
 
Partner säljare måste tilldelas rollen "hänvisnings administratör". Mer information finns i följande [behörigheter översikt) (Create-User-Accounts-and-set-Permissions).

4. Vilka fält måste konfigureras först i din CRM-miljö? 

• Kontrol lera att din valuta passar din plats och att den är korrekt i din CRM-miljö. • Ditt säljteam bör visas i din CRM-miljö som CRM-användare.

5. Vilka krav krävs för att skapa en automatisk miljö?

Om du vill använda Energis par miljön behöver du:

- En energi automatiserad licens krävs.
- Minst 1 GB lagring krävs.

6.  Behöver du en Dynamics 365-prenumeration för att använda Salesforce Connector-lösningen?

Salesforce Connector-lösningen är av typen "Dynamics Flow" som stöder synkronisering med andra CRM-system. Lösningen kräver inte att du har en Dynamics 365-instans eller en prenumeration. När du installerar Salesforce-lösningen kan det hända att en listruta med befintlig CD-miljö i företaget visas. Du måste välja den miljön. Om du får felet "vi kunde inte hitta en Dynamics 365-organisation som är ansluten till den inloggade användaren" måste du dessutom skapa en ny miljö för anslutnings tjänsten.

## <a name="questions-and-answers-about-configuration"></a>Frågor och svar om konfigurationen

1. Vad bör du göra om följande fel uppstår när du aktiverar flöden i en automatiserad plattform?

Fel: begäran till Azure Resource Manager misslyckades med felet: {"fel": {"Code": "WorkflowTriggerNotFound", "meddelande": "Det gick inte att hitta" e14d00f1-1fdf-4b1b-aaac-54a5064093d3 "-utlösaren för arbets flödet."}}. 

Följ dessa fel söknings steg:

- Ta bort CD-anslutningen och återskapa sedan CD-anslutningarna.
- Aktivera och inaktivera det underordnade flödet 
- Ta bort lösningen och installera sedan om lösningen. 

2.  Vad bör du göra om du kommer till fel meddelandet "logga in" när jag lägger till en partner Center-koppling i en automatiserad plattform?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Fel meddelande som kräver inloggning":::

Följ det här fel söknings steget:

- Använd dina partner Center-autentiseringsuppgifter för att logga in i Flow-miljön en gång (flow.microsoft.com).


3. Vad ska du göra om du får följande fel meddelande när du aktiverar Partner Center till CRM-flödet i en automatiserad plattform?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Fel meddelande som kräver inloggning":::

Följ dessa fel söknings steg:

- Aktivera följande två underordnade flöden innan du aktiverar Partner Center till CRM-flödet.
      - Partner Center till CRM – Helper (Insider Preview)
      - Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till CRM (Insider Preview)

4. Vad bör du göra när du inte kan lägga till anslutningar i flödet när du försöker redigera flödet?

Du lägger till anslutningar till flödet när flödet körs och du lägger till varje flöde separat.  Om dialog rutan för att lägga till anslutningar inte öppnas automatiskt när du redigerar flödet kan du redigera vart och ett av stegen och under stegen för flödena individuellt.

- Välj varje flöde och redigera dem individuellt.
- Expandera alla steg i flödet 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Fel meddelande som kräver inloggning":::

- Välj de steg där du ser en varnings ikon som uppmanar dig att associera anslutningar och lägga till anslutningar. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Fel meddelande som kräver inloggning":::


5. Vad ska jag göra om flödena för den samsälje referral Connector-lösningen inte aktive ras?

A. I energi spar läge måste du redigera flöden i följande ordning och uppdatera dem så att de använder rätt anslutningar:

- Partner Center – registrering av webhook (Insider Preview)
- Skapa Co-sälje referral-Salesforce till Partner Center (Insider Preview)
- Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till Salesforce (Insider Preview)
- Partner Center till Salesforce (Insider Preview)
- Salesforce till Partner Center (Insider Preview)
- Salesforce-möjlighet till Partner Center (Insider Preview)
- Salesforce Microsoft-lösningar till Partner Center (Insider Preview)

 B. För varje flöde väljer du alternativet **Kör endast användare** . Välj **Använd anslutning** i stället för att **tillhandahållas av endast körnings användare** .  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Fel meddelande som kräver inloggning":::


C. Aktivera följande flöden:

 - Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till Salesforce (Insider Preview)

- Salesforce till Partner Center (Insider Preview)

    
D. Aktivera alla återstående flöden.

E. I Flow Partner Center-webhook-registrering väljer du **Kör** . Ange **http-URL:** en från den första åtgärden i **partner Center till Salesforce** -flöde. Välj alla fyra alternativen under **händelser som ska registreras** och välj **Ja** för Skriv över.

## <a name="questions-and-answers-about-runmaintenance"></a>Frågor och svar om körning/underhåll

1. Hur felsöker jag om fel uppstår under automatisk flödes körning?

För att se till att dina energi scheman körs som du förväntar dig och Felsök fel under körningen, se [åtgärda flödes fel](/power-automate/fix-flow-failures).

2. Vad bör du göra om du ser referenser som inte har synkroniserats korrekt i Partner Center eller i en CRM-miljö?
 
Välj **granskning** för att fastställa status för referens synkroniseringen. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Fel meddelande som kräver inloggning":::

Se till att följande villkor är uppfyllda:

- Lösnings-ID tillhandahålls som en del av affärs möjligheten.

- Landskod för två bokstäver måste anges.

- När hjälp från Microsoft väljs för affärs möjligheten krävs kundens kontakt uppgifter.

3. Hur ser du till att en hänvisning synkroniseras i dubbelriktad riktning?

Gör så här:

- Partner leverantörer måste se till att de har aktiverat alternativet **Synkronisera med alternativet för partner Center** i avsnittet CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Fel meddelande som kräver inloggning" i Partner Center.

## <a name="next-steps"></a>Nästa steg

- [Hantera leads](manage-leads.md)
 
- [Hantera möjligheter till samförsäljning](manage-co-sell-opportunities.md)