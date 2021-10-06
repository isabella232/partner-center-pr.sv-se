---
title: Köpa Microsoft Azure reservationer för kunder
description: Lär dig hur du köper Azure-reservationer åt dina kunder i Partnercenter. Visar även marknader där Azure-reservationer inte är tillgängliga.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: 61ddb91e296436817e45ae0a2c3d9fe12b326f18
ms.sourcegitcommit: b78e85a0bc62e3536b067417cb3db7899cda4f97
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/06/2021
ms.locfileid: "129565299"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Köp Microsoft Azure reservationer åt dina kunder i Partnercenter

**Lämpliga roller:** Administratörsagent | Global | Supportagent | Försäljningsagentens | Administratör för användarhantering

Den här artikeln förklarar hur du köper Azure-reservationer åt dina kunder i Partnercenter. Den identifierar också marknader där Azure-reservationer inte är tillgängliga.
 
> [!NOTE]
> Den här artikeln gäller endast för partner i Molnlösningsleverantör-programmet (CSP). Kunder som använder andra typer av prenumerationer (till exempel betala enligt användning, enskilda prenumerationer, Microsoft-kundavtal- eller företagsavtal-prenumerationer) bör i stället läsa dokumentationen om [Azure-reservationer.](/azure/cost-management-billing/reservations)

## <a name="before-you-begin"></a>Innan du börjar

Granska viktig information nedan innan du köper Azure-reservationer åt dina kunder. (Vill du att kunderna ska kunna köpa sina egna Azure-reservationer från en tidigare Azure-prenumeration som du har köpt åt dem? Se [Ge kunder behörighet att köpa sina egna Azure-reservationer](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations).)

- Om och när kunden signerar den nya Microsoft-kundavtal (se Bekräfta kundens godkännande av [Microsoft-kundavtal](confirm-customer-agreement.md)) måste du köpa Azure-reservationer enligt Azure-planen. Mer information finns i Köpa [Azure-plan.](purchase-azure-plan.md)

- Kunderna måste redan ha en aktiv Azure-prenumeration innan du kan köpa reservationer åt dem
  
- Kostnader för programvaruprenumeration, SQL Database eller SUSE Linux-programvara, ingår inte i Priserna för Azure-reservationer

- Microsofts kommersiella priser för dig inkluderar inte skatter, såvida inte din plats är Brasilien. Om din plats är Brasilien inkluderar det kommersiella priset till dig lämpliga skatter

- Försäljnings- och supportavdelningen behöver explicit åtkomst till Azure-prenumerationen så att de kan köpa eller hantera den i Azure Portal- och filsupportbegäranden, inklusive för utbyten och återbetalningar, för kundens räkning  

- Om du är en indirekt leverantör och köper Azure-reservationer via Azure Portal, ärvs Partner of Record (indirekt återförsäljare) från den Azure CSP prenumeration som du väljer.

- Registrera partner för Azure-reservationer kan inte ändras efter köpet. Du kan avbryta den befintliga reservationen och köpa en ny med den nya partnern för posten.

- Om en kund vill överföra en Azure-prenumeration från Direkt eller EA till CSP överförs inte reservationer.

## <a name="azure-reservations-unavailable-markets"></a>Otillgängliga marknader för Azure-reservationer

> [!IMPORTANT]
> **Azure-reservationer är** inte tillgängliga på följande marknader:  
>  
> **Otillgängliga marknader (i alfabetisk ordning)**
>
> |A till Gi   | Gr till Pal  | Pap till Z |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | Åland     | Grönland     | Papua Nya Guinea     |
> | Amerikanska Samoa     | Grenada     | Pitcairn     |
> | Andorra     | Guadeloupe     | Réunion     |
> | Anguilla     | Guam     | Saba   |
> | Antarktis     | Guernsey     | Saint Barthélemy   |
> | Antigua och Barbuda       | Guinea     | Saint Lucia   |
> | Aruba       | Guinea-Bissau     | Saint Martin   |
> | Azerbajdzjan       | Guyana     | Saint-Pierre och Miquelon   |
> | Benin     | Haiti       | Saint Vincent och Grenadinerna     |
> | Bhutan     | Heard- och McDonaldöarna       | Samoa     |
> | Bonaire     | Isle of Man     | San Marino     |
> | Bouvetön     | Jan Mayen     | Séo Tomé och Prñncipe   |
> | Brittiska territoriet i Indiska Oceanen       | Jersey     | Seychellerna   |
> | Brittiska Jungfruöarna     | Kiribati       | Sierra Leone   |
> | Burkina Faso     | Kosovo     | Sint Eustatius     |
> | Burundi     | Laos     | Sint Maarten     |
> | Kambodja     | Lesotho     | Solomonöarna     |
> | Centralafrikanska Republiken     | Liberia     | Somalia     |
> | Tchad     | Madagaskar     | Sydgeorgien och Sydsandwichöarna     |
> | Kina     | Malawi     | Sydsudan     |
> | Julön     | Maldiverna     | StDirigering, Ascension, Tristan da Cunha     |
> | Kokosöarna     | Mali     | Surinam     |
> | Komorerna     | Marshallöarna     | Svalbard     |
> | Kongo     | Martinique     | Swaziland     |
> | Kongo (DR)     | Mauretanien     | Timor-Leste   |
> | Cooköarna     | Mayotte     | Togo   |
> | Djibouti     | Mikronesien     | Tokelau   |
> | Dominica     | Montserrat     | Tonga   |
> | Ekvatorialguinea     | Moçambique     | Turks- och Caicosöarna   |
> | Eritrea     | Myanmar     | Tuvalu   |
> | Falklandsöarna     | Nauru     | U.S. Outlying Islands   |
> | Franska Guyana     | Nya Kaledonien     | Vanuatu   |
> | Franska Polynesien     | Niger     | Vatikanstaten   |
> | Franska sydterritorierna     | Niue     | Wallis ochUna   |
> | Gabon     | Norfolkön     | Jemen   |
> | Gambia     | Nordmarianerna     |    |
> | Gibraltar     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Köp Azure-reservationer

Följ stegen nedan för att köpa Microsoft Azure reservationer åt dina kunder i Partnercenter. (Vill du att kunderna ska kunna köpa sina egna Azure-reservationer från en tidigare Azure-prenumeration som du har köpt åt dem? Se [Ge kunder behörighet att köpa sina egna Azure-reservationer](give-customers-permission.md).)

1. Välj **Kunder** på menyn i Partnercenter.  

2. På sidan **Kunder** hittar du den kund som vill köpa Azure-reservationer och väljer sedan nedåtpilen för att expandera kundens rad.  

3. Välj **Lägg till produkter** och välj sedan **Azure**. 

    a. Välj kundens marknadssegment i **listan** Segment.

    b. Välj **Reservationer** i **produktlistan** Typ.

    c. Välj den typ av reservation som kunden vill ha i **listan Reservationstyp.**

4. Azure-reservationer måste associeras med en aktiv Azure-prenumeration. Välj den kundprenumeration som du vill lägga till Azure-reservationer i från **listan Kundprenumeration.** 

   >[!IMPORTANT]
   >Om kunden inte redan har en aktiv Azure-prenumeration väljer du Azure för **att** lägga till en nu. 

5. Använd filtren för att hitta Azure-reservationer på virtuella datorer som uppfyller kundens krav.  

6. När du har hittat de reservationer som du vill köpa anger du  antalet reserverade instanser som kunden behöver i Kvantitet och väljer sedan Lägg **till i kundvagn.**  

7. Upprepa steg 5 och 6 tills du har lagt till alla nödvändiga objekt i ordern. Välj **Granska** för att kontrollera att beställningen är korrekt.  

8. På sidan **Granska dina beställningar** kan du: 

    - Verifiera eller ändra antalet reserverade instanser.

    - Välj reservationens omfång. Reservationens omfång kan omfatta en prenumeration eller flera prenumerationer (delat omfång). Om du omfångsbefattningar reservationen till en enda prenumeration tillämpas reservationsrabatten endast på den här prenumerationen. Om du väljer delad tillämpas reservationsrabatten på alla prenumerationer i kundens faktureringskontext. 

      > [!NOTE] 
      > Om du väljer att begränsa reservationens omfång till en enda Azure-prenumeration kan du behöva öka prenumerationens vCPU-kvot. Om du vill öka prenumerationens vCPU-kvot måste du skapa en supportbegäran i Azure Portal. Följ anvisningarna [i det här avsnittet](/azure/azure-supportability/resource-manager-core-quotas-request) för att skapa begäran. 

      > [!NOTE]   
      > Om kunden omfattas av Azure-planen **ställs** omfånget in på **Delat** vid tidpunkten för köpet. Detta kan ändras senare.

    - Om du är leverantörspartner väljer du den återförsäljare som du vill associera med produkten.
    
    - Om din Azure-reservation stöder alternativet Faktureringsplan kan du välja faktureringsfrekvens per månad från den nedrullningsbara menyn. 
    - Om din Azure-reservation inte stöder alternativet Faktureringsplan används faktureringsfrekvensen som standard en gång. 

9. Välj **Köp** för att köpa beställningen. Information om din beställning, inklusive ordernummer, visas på **sidan** Bekräfta. Välj **Klar** för att gå till **sidan Orderhistorik.** 

10. Om du vill hantera kundens reservation i Azure Portal du kunden på sidan **Kunder** och väljer sedan nedåtpilen för att expandera kundens rad. Välj **Microsoft Azure Hanteringsportal** för att öppna kundens post i Azure Portal.

## <a name="next-steps"></a>Nästa steg

|**För information om**   |**Läs detta**    |
|:-----------------------------|:-----------------|
|Översikt över Azure-reservationer i CSP  | [Sälja Microsoft Azure reserverade instanser](azure-reservations.md) |
|Hantera Azure-reservationer i Partnercenter | [Hantera Azure-reservationer i Partnercenter](azure-reservations-manage.md)
|Fastställ rätt VM-storlek och verifiera kundens VM-användning   |[VM-storlek för maximal användning av Azure-reservationer](azure-usage.md)   |
|Köpa Azure-reservationer med partnercenter-API:et | [Köp Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) i utvecklardokumentationen för Partnercenter   |
|Ge kunderna tillstånd att köpa sina egna Azure-reservationer  | [Ge kunderna behörighet att köpa sina egna Azure-reservationer](give-customers-permission.md)  |
