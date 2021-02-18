---
title: Överför Azure-prenumeration till en annan partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du ändrar program partner för Cloud Solution Provider som är associerad med kundens Azure-prenumerationer.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: b9058b00708e0ed745c7d6343dfd9c04382cfa9e
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645664"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Läs om hur du överför en Azure-prenumeration för en kund till en annan partner

**Gäller för**

- Välkommen till Partnercenter för Microsoft Cloud for US Government
- Partner Center för Microsoft Global Cloud
- Partner i CSP-programmet (Cloud Solution Provider)

I den här artikeln beskrivs hur en kund kan byta Microsoft Azure-tjänster från en leverantör av moln lösningar till en annan.

Följ dessa manuella steg om du vill byta en kunds Azure-tjänster eller prenumerationer till en annan partner. Både partnern och kunden måste slutföra stegen.

>[!Note]  
>För närvarande kan endast direkta eller indirekta leverantörer överföra prenumerationer.
>Du kan inte ändra partner för prenumerationer på moln lösnings leverantörer som är associerade med Azure plan, Office 365, Enterprise Mobility Suite eller Microsoft Dynamics CRM-prenumerationer.

## <a name="switch-partners-for-azure-subscriptions"></a>Byta partner för Azure-prenumerationer

1. För att överföra en Azure-prenumeration till en ny partner, måste kunden starta processen och kontakta sin nuvarande partner av posten i skriftlig form.

   >[!Note]
   > Det är den aktuella partnerns ansvar att skapa tjänst biljetten som initierar överförings processen. Microsoft kan inte ingripa för kundens räkning eller den nya partnern. Kunden bör planera att samar beta med den aktuella partnern för att få över gången att gå smidigt.

2. Partnern för prenumerationen måste utföra följande uppgifter:

   Skapa en Azure Service-biljett från Partner Center för att begära en prenumerations överföring:

   1. Från menyn Partner Center väljer du **kunder**, väljer din kund i listan och väljer sedan **tjänst hantering**. 

   2. Under avsnittet **support biljetter** väljer du List rutan **New Ticket** och väljer **Microsoft Azure**.
   
   3. Välj **nytt support ärende** från [Azure Portal](https://portal.azure.com).
   
   4. I steg 1 väljer du **prenumerations hantering** som typ av ärende, anger det PRENUMERATIONS-ID som du vill överföra och väljer sedan **Cloud Solution Provider** som support avtal.
   
   5. I steg 2 väljer du **C-minimal påverkan** och väljer **andra allmänna frågor** som problem typ.
   
   6. Hämta [överförings formuläret för CSP-prenumeration](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC).

3. Partnern för prenumerationen: Fyll i [formuläret för prenumerations överföring i CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC), signera det och skicka det till kunden. 

   Du behöver följande information för att fylla i formuläret:

   - Den aktuella partnerns kontakt uppgifter och Microsoft ID. I menyn Partner Center väljer du **konto inställningar** &gt; **organisations profil** och använder **Microsoft ID**, **organisations namn** och **adress** som visas där.

   - Kundens Microsoft-ID. I menyn Partner Center väljer du **kunder** och expanderar sedan kund listan för att se deras **Microsoft-ID**.

   - Prenumerations-ID som ska överföras. I den expanderade kund listan väljer du **Visa prenumerationer** och expandera sedan den valda prenumerationen för att se **prenumerations-ID: t**.

   >[!Note]
   >Överföring av prenumerations resultat i två prenumerations-ID: n som visas på sidan **Redigera prenumeration** för den överförda prenumerationen: **1**– prenumerations-ID för partner Center används i fakturerings syfte. **2**– det ursprungliga ID: t för Azure-prenumerationen behålls och visas i Partner Center och i hanterings portalen för Azure. Det här ID: t visas i din rekognoseringar-fil.  **När du loggar support biljetter måste du använda båda ID: na.**

4. Prenumerationens kund och nya partner:

   Granska formuläret, Fyll i information om den nya partnern och signera den. Bekräfta att den nya kunden har ett kontrakts avtal på plats. Skicka tillbaka formuläret till den aktuella partnern av posten.

   *Viktigt*: om den nya CSP-partnern inte har en åter försäljares relation med kunden måste han eller hon upprätta en innan prenumerationen överförs. [Du hittar information om hur du gör detta här](request-a-relationship-with-a-customer.md).

   >[!Note]
   >Den nya CSP-partnern och kund klienten måste vara i samma land. 

5. Aktuell partner:

   Se till att formuläret innehåller kontakt information för båda partner administratörerna. Microsoft Support kommer att kontakta båda administratörerna för att verifiera överföringen. Kontrol lera att du har alla tre signaturer. Använd sedan alternativet för **fil uppladdning** för att bifoga det färdiga formuläret till din befintliga tjänstbegäran. En Microsoft-support tekniker kommer tillbaka till dig inom åtta arbets timmar för att validera inbetalnings-och slut för ande.

6. Ny partner:

   Uppdatera inställningarna för Azure-prenumerationen för att ta bort den gamla partnern från kontot. Du kan se vilka roll tilldelningar som är etablerade genom att köra två PowerShell-cmdletarna.

   - Lägg till den nya partnern som åter försäljare för kontot:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > Kundens **klient-ID** visas i Partner Center som kundens **Microsoft-ID**. Om du vill hitta Microsoft ID (klient-ID) för en specifik kund loggar du in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard). Välj sedan **kunder** på menyn. Leta upp kunden i listan. Välj nedpilen för att expandera kundens lista. Du kommer att se information om kundens *domän namn* och kundens **Microsoft-ID**. Använd det 16-siffriga **Microsoft-ID: t** i PowerShell-kommandot.

   - Visa roller för kontot, inklusive tidigare CSP-partner:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Ta bort föråldrade åtkomst behörigheter

   - I menyn Partner Center väljer du **kunder**.
   - Leta upp kunden i listan. Välj företagets namn genom att välja (dubbelklicka). Då öppnas sidan kund **prenumerationer** .
   - Välj **tjänst hantering** på menyn kund information.
   - Under **Microsoft Azure** klickar du på länken för att gå till **Microsoft Azure-hanteringsportal**.

## <a name="next-steps"></a>Nästa steg

- Hämta [överförings formuläret för CSP-prenumeration](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

- Läs mer om [stöd för flera partner](multipartner.md).

- [stöd för flera partner](multipartner.md).
- [stöd för flera kanaler](multichannel.md).
- [Överföra Azure-prenumerationer](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)