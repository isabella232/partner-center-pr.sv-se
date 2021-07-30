---
title: Överföra En Azure-prenumeration till en annan partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Lär dig hur du ändrar Molnlösningsleverantör partner som är associerad med en kunds Azure-prenumerationer.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/21/2021
ms.openlocfilehash: c1bc82e852c6777bc9e8c01a33b0976269e31b2f
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114843603"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Läs om hur du överför en Azure-prenumeration för en kund till en annan partner

**Gäller för:** Partner Center-| Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller:** Global administratör

Den här artikeln beskriver hur en kund kan byta Microsoft Azure tjänster från en Molnlösningsleverantör (CSP) till en annan när de har köpt det tidigare Azure-erbjudandet i CSP.

Efter fas 1 av de ändringar vi gör i det tidigare Azure-erbjudandet i [CSP](https://go.microsoft.com/fwlink/p/?linkid=2164140)kan partnern fortsätta att göra ändringar i det tidigare Azure-erbjudandet (MS-AZR-0145p) för alla befintliga återförsäljarrelationer mellan partner och kunder i CSP-programmet om kunden redan har köpt det. För alla befintliga återförsäljarrelationer mellan partner och kunder gäller att om kunden inte har köpt det tidigare Azure-erbjudandet tidigare, kan partnern bara köpa det nya Azure-erbjudandet.

- Om både den aktuella och framtida **partnern** har aktiva tidigare Azure-erbjudandeprenumerationer med en kund fortsätter det tidigare Azure-erbjudandet (MS-AZR-0145p) som beskrivs i det här dokumentet mellan den aktuella och framtida partnern att vara tillgängligt efter fas 1 så länge båda partnerna har aktiva tidigare Prenumerationer på Azure-erbjudanden. Den här överföringsfunktionerna avslutas antingen när en framtida partner inte längre har några aktiva tidigare Azure-erbjudandeprenumerationer eller när det tidigare Azure-erbjudandet (MS-AZR-0145p) i CSP dras tillbaka permanent i fas 3.

   > [!NOTE]
   > Det finns inga automatiserade verktyg för det här scenariot och nedanstående process måste utnyttjas.

- Om endast den aktuella partnern har en kund med ett aktivt tidigare **Azure-erbjudande (MS-AZR-0145p)** och den framtida partnern inte gör det, är överföringen av det tidigare Azure-erbjudandet mellan partner inte längre möjlig efter fas 1. Eftersom den framtida partnern inte kan skapa ett tidigare Azure-erbjudande (MS-AZR-0145p) för kunden, skulle den här överföringen inte aktiveras. I det här fallet kan det här övergångsverktyget användas för att flytta kundens Azure-prenumeration mellan partner i CSP samtidigt som det konverteras till en ny Azure-erbjudandeprenumeration.

Om du vill byta en kunds Azure-tjänster eller prenumerationer till en annan partner med det tidigare Azure-erbjudandet (MS-AZR-0145p) följer du dessa manuella steg. Både partnern och kunden måste slutföra stegen.

> [!NOTE]  
> För närvarande kan endast direkta eller indirekta leverantörer överföra prenumerationer.
> Du kan inte byta partner för Molnlösningsleverantör prenumerationer som är associerade med Azure-prenumeration, Office 365, Enterprise Mobility Suite eller Microsoft Dynamics CRM prenumerationer.

## <a name="transfer-azure-subscriptions-to-another-partner-with-the-previous-azure-offer"></a>Överföra Azure-prenumerationer till en annan partner med det tidigare Azure-erbjudandet

1. Om du vill överföra en Azure-prenumeration till en ny partner med det tidigare Azure-erbjudandet måste kunden starta processen och kontakta sin nuvarande partner med posten genom att skriva.

   > [!NOTE]
   > Det är den aktuella partnerns ansvar att skapa tjänstbiljetten som initierar överföringsprocessen. Microsoft kan inte ingriper åt kunden eller den nya partnern. Kunden bör planera att samarbeta med den aktuella partnern för att övergången ska gå smidigt.

2. Partnern för prenumerationen måste utföra följande uppgifter:

   Skapa en Azure-tjänstbiljett från Partnercenter för att begära en prenumerationsöverföring:

   1. I menyn i Partnercenter väljer **du Kunder,** väljer kunden i listan och väljer sedan **Tjänsthantering.**
   2. Under avsnittet **Supportärenden** väljer du **listrutan Ny** biljett och väljer **Microsoft Azure**.
   3. Från [Azure Portal](https://portal.azure.com)väljer du **Ny supportbegäran.**
   4. I steg 1 väljer du **Prenumerationshantering** som problemtyp, anger det prenumerations-ID som du vill överföra och väljer **Molnlösningsleverantör** som supportplan.
   5. I steg 2 väljer du **C-Minimal påverkan** och **väljer Andra allmänna** frågor som problemtyp.
   6. Ladda ned [formuläret CSP Subscription Transfer (Överföring av CSP-prenumeration).](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)

3. Partnern för prenumerationen: Fyll i formuläret [Överföring av CSP-prenumeration,](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)signera den och skicka den sedan till kunden. 

   För att fylla i formuläret behöver du följande information:

   - Den aktuella partnerns kontaktuppgifter och Microsoft-ID. I menyn i Partnercenter väljer du **Kontoinställningar** &gt; **Organisationsprofil** och använder **Microsoft-ID,** **Organisationsnamn** och **Adress som** visas där.
   - Kundens Microsoft-ID. I menyn i Partnercenter väljer du **Kunder** och expanderar sedan kundens lista för att se kundens **Microsoft-ID.**
   - Prenumerations-ID:t som ska överföras. I den expanderade kundlistan väljer du Visa prenumerationer och **expanderar** sedan den valda prenumerationen för att se **Prenumerations-ID.**

   > [!NOTE]
   > Överföring av en prenumeration resulterar i två prenumerations-ID:n som visas på sidan Redigera prenumeration för den överförda prenumerationen: **1**– Prenumerations-ID för Partnercenter används i faktureringssyfte.  **2**– Det ursprungliga Azure-prenumerations-ID:t behålls och visas i Partnercenter samt i Azure-hanteringsportalen. Detta ID visas i rekognoseringsfilen.  **När du loggar supportärenden måste du använda båda-ID:erna.**

4. Kunden och den nya partnern för prenumerationen:

   Granska formuläret, fyll i information om den nya partnern och signera det. Bekräfta att den nya kunden har ett avtal på plats. Skicka formuläret tillbaka till den aktuella partnern för posten.

   *Viktigt!* Om den nya CSP-partnern inte har en återförsäljarrelation med kunden måste den upprättas innan prenumerationen överförs. [Du hittar information om hur du gör detta här.](request-a-relationship-with-a-customer.md)

   > [!NOTE]
   > Den nya CSP-partnern och kundklientorganisationen måste finnas i samma land. 

5. Aktuell partner:

   Kontrollera att formuläret innehåller kontaktinformation för båda partneradministratörerna. Microsoft Support båda administratörerna för att verifiera överföringen. Kontrollera att du har alla tre signaturerna. Använd sedan alternativet **Fil Upload** för att bifoga det ifyllda formuläret till din befintliga tjänstbegäran. En Microsoft-supporttekniker kommer tillbaka till dig inom åtta timmar för att verifiera kvitto och slutförande.

6. Ny partner:

   Uppdatera inställningarna för Azure-prenumerationen för att ta bort den gamla partnern från kontot. Om du vill se vilka rolltilldelningar som har etablerats kör du två PowerShell-kommandon.

   - Lägg till den nya partnern som återförsäljare på kontot:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     > [!NOTE]
     > Kundens **klientorganisations-ID** visas i Partnercenter som kundens **Microsoft-ID.** Om du vill hitta Microsoft-ID :t (klient-ID) för en specifik kund loggar du in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard) Välj sedan **Kunder** på menyn. Leta upp kunden i listan. Välj nedåtpilen för att expandera kundens lista. Du ser information om kundens domännamn *och kundens* **Microsoft-ID.** Använd det 16-siffriga **Microsoft-ID:t** i PowerShell-kommandot.

   - Visa roller för kontot, inklusive tidigare CSP-partner:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Ta bort inaktuella åtkomstbehörigheter:

   1. I menyn i Partnercenter väljer du **Kunder.**
   1. Leta upp kunden i listan. Välj (dubbelklicka på) företagets namn. Den här åtgärden öppnar sidan **Kundprenumerationer.**
   1. I menyn med kundinformation väljer du **Tjänsthantering.**
   1. Under **Microsoft Azure** väljer du **Microsoft Azure Hanteringsportal** länken.

## <a name="next-steps"></a>Nästa steg

- [Överföra Azure-prenumerationer](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)
- [Överföra Azure-prenumerationer under en Azure-plan](transfer-azure-subscriptions-under-azure-plan.md)
- Ladda ned [formuläret för överföring av CSP-prenumeration](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)
- Läs mer [om stöd för flera partner](multipartner.md)
- Läs mer [om stöd för flera kanaler](multichannel.md)
