---
title: Överföra En Azure-prenumeration till en annan partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du ändrar Molnlösningsleverantör programpartner som är associerad med en kunds Azure-prenumerationer.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: b21bfcae4472763c19481ad506ae1c72d238e8f0
ms.sourcegitcommit: 26e6b470756aa9c1b3b0b919301b0eb38a335a52
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/26/2021
ms.locfileid: "108002916"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Läs om hur du överför en Azure-prenumeration för en kund till en annan partner

**Gäller för**

- Välkommen till Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller**

- Global administratör

Den här artikeln beskriver hur en kund kan byta Microsoft Azure tjänster från en Molnlösningsleverantör (CSP) till en annan.

Följ dessa manuella steg om du vill byta en kunds Azure-tjänster eller prenumerationer till en annan partner. Både partnern och kunden måste slutföra stegen.

>[!Note]  
>För närvarande kan endast direkta eller indirekta leverantörer överföra prenumerationer.
>Du kan inte byta partner för Molnlösningsleverantör prenumerationer som är associerade med Azure-plan, Office 365, Enterprise Mobility Suite eller Microsoft Dynamics CRM-prenumerationer.

## <a name="switch-partners-for-azure-subscriptions"></a>Byta partner för Azure-prenumerationer

1. För att kunna överföra en Azure-prenumeration till en ny partner måste kunden starta processen och kontakta sin aktuella partner med en post genom att skriva.

   >[!Note]
   > Det är den aktuella partnerns ansvar att skapa tjänstbiljetten som initierar överföringsprocessen. Microsoft kan inte ingriper för kundens eller den nya partnerns räkning. Kunden bör planera att samarbeta med den aktuella partnern för att övergången ska gå smidigt.

2. Partnern för prenumerationen måste utföra följande uppgifter:

   Skapa en Azure-tjänstbiljett från Partnercenter för att begära en prenumerationsöverföring:

   1. I menyn i Partnercenter väljer **du Kunder,** väljer kunden i listan och väljer sedan **Tjänsthantering.**

   2. Under avsnittet **Supportärenden** väljer du **listrutan Nytt** ärende och väljer **Microsoft Azure**.
   
   3. Från den [Azure Portal](https://portal.azure.com)väljer du **Ny supportbegäran.**
   
   4. I steg 1 väljer du **Prenumerationshantering** som problemtyp, anger det prenumerations-ID som du vill överföra och väljer **Molnlösningsleverantör** som supportplan.
   
   5. I steg 2 väljer du **C-Minimal påverkan** och **väljer Andra allmänna** frågor som problemtyp.
   
   6. Ladda ned [formuläret CSP Subscription Transfer (Överföring av CSP-prenumeration).](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)

3. Partnern för prenumerationen: Fyll i formuläret [Överföring av CSP-prenumeration,](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)signera den och skicka den sedan till kunden. 

   Om du vill fylla i formuläret behöver du följande information:

   - Den aktuella partnerns kontaktuppgifter och Microsoft-ID. I menyn i Partnercenter väljer du **Kontoinställningar** &gt; **Organisationsprofil** och använder **Microsoft-ID,** **Organisationsnamn** och **Adress som** visas där.

   - Kundens Microsoft-ID. I menyn i Partnercenter väljer du **Kunder** och expanderar sedan kundens lista för att se kundens **Microsoft-ID.**

   - Prenumerations-ID:t som ska överföras. I den expanderade kundlistan väljer du Visa prenumerationer och **expanderar** sedan den valda prenumerationen för att se **Prenumerations-ID.**

   >[!Note]
   >Överföring av en prenumeration resulterar i två prenumerations-ID:n som visas på sidan Redigera prenumeration för den överförda prenumerationen: **1**– Prenumerations-ID för Partnercenter används i faktureringssyfte.  **2**– Det ursprungliga Azure-prenumerations-ID:t behålls och visas i Partnercenter samt i Azure-hanteringsportalen. Detta ID visas i rekognoseringsfilen.  **När du loggar supportärenden måste du använda båda-ID:erna.**

4. Kunden och den nya partnern för prenumerationen:

   Granska formuläret, fyll i information om den nya partnern och signera det. Bekräfta att den nya kunden har ett avtal på plats. Skicka formuläret tillbaka till den aktuella partnern för posten.

   *Viktigt!* Om den nya CSP-partnern inte har en återförsäljarrelation med kunden måste den upprättas innan prenumerationen överförs. [Du hittar information om hur du gör detta här.](request-a-relationship-with-a-customer.md)

   >[!Note]
   >Den nya CSP-partnern och kundklientorganisationen måste finnas i samma land. 

5. Aktuell partner:

   Kontrollera att formuläret innehåller kontaktinformation för båda partneradministratörerna. Microsoft Support båda administratörerna för att verifiera överföringen. Kontrollera att du har alla tre signaturerna. Använd sedan alternativet **Filuppladdning** för att koppla det ifyllda formuläret till din befintliga tjänstbegäran. En Microsoft-supporttekniker kommer tillbaka till dig inom åtta timmar för att verifiera kvitto och slutförande.

6. Ny partner:

   Uppdatera inställningarna för Azure-prenumerationen för att ta bort den gamla partnern från kontot. Om du vill se vilka rolltilldelningar som har etablerats kör du två PowerShell-kommandon.

   - Lägg till den nya partnern som återförsäljare på kontot:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > Kundens **klientorganisations-ID** visas i Partnercenter som kundens **Microsoft-ID.** Om du vill hitta Microsoft-ID:t (klient-ID) för en specifik kund loggar du in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard) Välj sedan **Kunder** på menyn. Leta upp kunden i listan. Välj nedåtpilen för att expandera kundens lista. Du ser information om kundens domännamn *och kundens* **Microsoft-ID.** Använd det 16-siffriga **Microsoft-ID:t** i PowerShell-kommandot.

   - Visa roller för kontot, inklusive tidigare CSP-partner:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Ta bort inaktuella åtkomstbehörigheter:

   - I menyn i Partnercenter väljer du **Kunder.**
   - Leta upp kunden i listan. Välj (dubbelklicka på) företagets namn. Den här åtgärden öppnar sidan **Kundprenumerationer.**
   - I menyn med kundinformation väljer du **Tjänsthantering.**
   - Under **Microsoft Azure** väljer du länken för att gå till **Microsoft Azure-hanteringsportal**.

## <a name="next-steps"></a>Nästa steg

- Ladda ned [formuläret CSP Subscription Transfer (Överföring av CSP-prenumeration).](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA)

- Lär dig [mer om stöd för flera partner.](multipartner.md)

- [stöd för flera partner.](multipartner.md)
- [stöd för flera kanaler.](multichannel.md)
- [Överföra Azure-prenumerationer](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)