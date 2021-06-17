---
title: Felsöka anslutningsappar för hänvisningar till säljförsäljning
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Få svar på vanliga frågor om hur du använder anslutningsappar för säljförsäljning. Läs dessa vanliga frågor och svar om hur du felsöker anslutningsappar för säljförsäljning.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: bb7a227624c548a29046b80d3bd5fa363a4aee2f
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276946"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Felsöka anslutningsappar för hänvisningar till säljförsäljning

**Gäller för**: Dynamics 365 CRM | Salesforce CRM

**Lämpliga roller:** Referensadministratörsroller | Systemadministratör eller systemanpassare för CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Frågor och svar om förutsättningar

1. Kan du använda en anslutningsapp för utvärderingsversionen av anslutningsappar för säljförsäljning för din miljö?

Om du använder test-/mellanlagringsmiljön kan du välja utvärderingslösning. Den betalda versionen av anslutningsapparna är tillgänglig i AppSource på US$ 15 per månad. Med den betalda anslutningen får du 10 000 API-anrop per dag. Anslutningsapparna är omslutningar ovanpå Partner Center-hänvisnings-API:er. När anslutningslösningarna körs för en **skapa-** eller **uppdateringshändelse** på antingen Partner Center- eller CRM-sidan görs ett API-anrop.

2. Vilken roll behöver du för att skapa avsnitt i CRM-miljön?

Användare som är systemadministratörer eller systemanpassare kan tillämpa ändringar för alla. Alla appanvändare kan dock anpassa systemet och även dela vissa av sina anpassningar med andra. 

3. Behöver partnerförsäljare särskilda roller för att arbeta i Partnercenter?
 
Partner säljare måste tilldelas rollen "Referensadministratör". Mer information finns i Översikt [över behörigheter.](create-user-accounts-and-set-permissions.md)

4. Vilka fält måste konfigureras först i crm-miljön? 

• Kontrollera att din valuta är lämplig för din plats och är korrekt i DIN CRM-miljö. • Säljteamet bör anges som CRM-användare i din CRM-miljö.

5. Vilka förutsättningar krävs för att skapa Power Automate miljön?

Om du vill Power Automate miljön behöver du:

- En Power Automate licens krävs.
- Minst 1 GB lagringsutrymme krävs.

6.  Behöver du en Dynamics 365-prenumeration för att använda Salesforce Connectors-lösningen?

Salesforce Connector-lösningen är av typen "Dynamics Flow" som stöder synkronisering med andra CRM-system. Lösningen kräver inte att du har en Dynamics 365-instans eller en prenumeration. När du installerar Salesforce-lösningen kan en listrutan med befintlig CDS-miljö i ditt företag visas. Du måste välja den miljön. Om du får felmeddelandet "Det gick inte att hitta en Dynamics 365-organisation som är ansluten till den inloggade användaren" måste du dessutom skapa en ny miljö för anslutning.

## <a name="questions-and-answers-about-configuration"></a>Frågor och svar om konfiguration

1. Vad ska du göra om du får följande fel när du aktiverar flöden i Power Automate Platform?

Fel: Begäran till Azure Resource Manager misslyckades med felet: "{"error":{"code":"WorkflowTriggerNotFound","message":"Arbetsflödet "e14d00f1-1fdf-4b1b-aaac-54a5064093d3" utlösaren "manual" kunde inte hittas."}}'. 

Följ dessa felsökningssteg:

- Ta bort CDS-anslutningen och återskapa sedan CDS-anslutningarna.
- Inaktivera och aktivera det underordnade flödet 
- Ta bort lösningen och installera sedan om lösningen. 

2.  Vad ska du göra om du får felet "Logga in" när du lägger till en Partner Center-anslutning i Power Automate Platform?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Felmeddelande som kräver inloggning.":::

Följ det här felsökningssteget:

- Använd dina autentiseringsuppgifter för Partnercenter för att logga in i flödesmiljön en gång (flow.microsoft.com).


3. Vad ska du göra om du får följande fel när du aktiverar PartnerCenter till CRM-flödet i Power Automate Platform?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Felmeddelande som kräver uppdateringar.":::

Följ dessa felsökningssteg:

- Aktivera följande två underordnade flöden först innan du aktiverar Partnercenter för CRM-flödet.
      - Partner Center till CRM – Helper (Insider Preview)
      - Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)

4. Vad ska du göra när du inte kan lägga till anslutningar till flödet när du försöker redigera flödet?

Du lägger till anslutningar till flödet medan flödet körs och lägger till i varje flöde separat.  Om dialogrutan för att lägga till anslutningar inte öppnas automatiskt när du redigerar flödet kan du redigera vart och ett av stegen och understegen för flödena individuellt.

- Markera varje flöde och redigera dem individuellt.
- Expandera alla steg i flödet 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Steg som behöver anslutningar.":::

- Välj de steg där du ser en varningsikon där du uppmanas att associera anslutningar och lägga till anslutningar. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Redigera flödet steg för steg.":::


5. Vad ska du göra om flödena i lösningen anslutningsappar för säljförsäljning inte är på?

A. I Power Automate måste du redigera flöden i följande ordning och uppdatera dem så att de använder rätt anslutningar:

- Registrering av Webhook i Partnercenter (insiderförhandsvisning)
- Skapa hänvisning till säljförsäljning – Salesforce till Partner Center (insiderförhandsvisning)
- Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)
- Partner Center till Salesforce (insiderförhandsvisning)
- Salesforce till Partner Center (Insider Preview)
- Salesforce Opportunity to Partner Center (Insider Preview)
- Salesforce Microsoft Solutions to Partner Center (Insider Preview)

 B. För vart och ett av flödena väljer **du alternativet Kör endast** användare. Välj **Använd anslutning i** stället för Tillhandahålls av den **körbaserade användaren**.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Så här aktiverar du ett flöde.":::


C. Aktivera dessa nedanstående flöden:

 - Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)

- Salesforce till Partner Center (Insider Preview)

    
D. Aktivera alla återstående flöden.

E. I flödet Partner Center Webhook Registration (Partnercenter-webhookregistrering) väljer **du Kör**. Ange **HTTP-URL:en** från den första åtgärden **i Partnercenter till Salesforce-flödet.** Välj alla fyra alternativen under **Händelser för att** registrera dig och **välj** Ja för Overwrite (Skriva över).

## <a name="questions-and-answers-about-runmaintenance"></a>Frågor och svar om körning/underhåll

1. Hur felsöker du fel Power Automate körningen av flödet?

Information om hur du Power Automate körs som förväntat och felsöker fel under körningen finns i Åtgärda [flödesfel.](/power-automate/fix-flow-failures)

2. Vad ska du göra om du ser referenser som inte synkroniseras korrekt i Partner Center eller CRM-miljön?
 
Välj Granska för att fastställa statusen för **referenssynkronisering.** 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Så här synkroniserar du referenser.":::

Kontrollera att följande villkor är uppfyllda:

- Lösnings-ID anges som en del av affärsmöjligheten.

- Landskod med två bokstäver krävs.

- När hjälp från Microsoft har valts för affärsmöjligheten krävs kundkontaktinformation.

3. Hur ser du till att en hänvisning synkroniseras i dubbelriktad riktning?

Gör följande:

- Partnerförsäljare måste se till att de har aktiverat alternativet **Synkronisera med Partnercenter** i CRM-avsnittet.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Kontrollera att du har aktiverat Synch.":::

- Säljare måste ange intäkter och slutdatum när de kvalificerar en lead.

- Om CRM-ID anges  i  fasen för att skapa eller uppdatera säljförsäljning, men en lead-affärsmöjlighet med det ID:t inte hittas i CRM, ignoreras uppdatering eller skapa.

- Se till att fältet hänvisningsvaluta har konfigurerats i Salesforce-miljön. 

4. Vad ska du göra om anslutningsappen kopplas från och du missar en hänvisningssynkronisering.?

Följande är några av de alternativ som du kan prova:

- Kontrollera om användarnamnet eller lösenordet har upphört att gälla för Partnercenter-användaren med referensadministratörsroller.

- Du kan gå till den icke-synkroniserade affärsmöjligheten, göra en mindre uppdatering och se om hänvisningen har synkroniserats.

- Om flödena har körts och misslyckats väljer du flödet och skickar om körningen som misslyckades.

5. Vad ska du göra när du får felmeddelanden om nekad åtkomst?

Kontrollera att rätt roller finns

- Referensadministratörsroll för Partner Center-säljare 
 
- Systemadministratörs- eller systemanpassarroll på din CRM-instans

- Kontrollera att Power Automate flödeskontoanvändare loggar in https://flow.microsoft.com på minst en gång i förväg

6. Vad ska du göra om **du** ser att landskoden för kundkontot saknas när du skapar en möjlighet till säljförsäljning?

Du måste lägga till ISO-landskoden med två bokstäver till kundkontot i CRM.

7. Vad ska du göra om du ser felet att **lösnings-ID krävs när** du skapar en möjlighet till säljförsäljning?

För att kunna skapa en hänvisning till säljförsäljning behöver du en lösning som är redo för microsofts säljförsäljning. 

8. Vad ska du göra när du ser möjligheter till säljförsäljning i Partnercenter som inte synkroniseras med CRM trots att det inte finns några flödesfel?

Gör följande:

- När du har skapat ett nytt säljavtal i Partnercenter kontrollerar du om Partner Center till Dynamics 365-flöde anropas (det kan anropas flera gånger).

- Om flödet anropas kontrollerar du alla anropade flöden och identifierar den flödeskörning som uppdaterar CRM. Du kan följa åtgärderna och kontrollera om CRM har uppdaterats eller om ett problem har uppstått.

- Markera **Nytt avtal i** Partnercenter för att se om det fylls med CRM-ID.

- Kontrollera att avtalet inte har stängts av misstag som Won **(Vunnit)** **eller Lost (Förlorad)** i Partnercenter.

## <a name="next-steps"></a>Nästa steg

- [Hantera leads](manage-leads.md)
 
- [Hantera möjligheter till samförsäljning](manage-co-sell-opportunities.md)
