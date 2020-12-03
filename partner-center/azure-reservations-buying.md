---
title: Köp Microsoft Azure reservationer för kunder
description: Lär dig hur du köper eller köper Azure-reservationer för dina kunders räkning i Partner Center. Visar även marknader där Azure-reservationer inte är tillgängliga.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: 0e81a9561f3749aab281bb4ebd7cd0c38540ff31
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534615"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Köp Microsoft Azure reservationer för dina kunders räkning i Partner Center

**Lämpliga roller**

- Administratörs agent
- Global administratör
- Support agent
- Försäljnings agent
- Administratör för användar hantering

Den här artikeln beskriver hur du köper eller köper Azure-reservationer för dina kunders räkning i Partner Center. Den identifierar även marknader där Azure-reservationer inte är tillgängliga.
 
> [!NOTE]
> Den här artikeln gäller endast partner i Cloud Solution Provider (CSP)-programmet. Kunder som använder andra typer av prenumerationer (t. ex. betala per användning, enskilda, Microsoft-kundavtal eller Enterprise-avtal prenumerationer) bör i stället läsa [denna dokumentation om Azure-reservationer](/azure/cost-management-billing/reservations).

## <a name="before-you-begin"></a>Innan du börjar

Läs den viktiga informationen nedan innan du köper Azure-reservationer åt dina kunder. (Vill du att kunderna ska kunna köpa sina egna Azure-reservationer från en tidigare Azure-prenumeration som du har köpt för dem? Se [ge kunderna tillstånd att köpa sina egna Azure-reservationer](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations).)

- Om och när kunden registrerar det nya Microsofts kund avtal (se [bekräfta kund godkännande av Microsofts kund avtal](confirm-customer-agreement.md)) måste du köpa Azure-reservationer i Azure-planen. Mer information finns i [köpa Azure-plan](purchase-azure-plan.md).

- Kunderna måste redan ha en aktiv Azure-prenumeration innan du kan köpa reservationer för deras räkning
  
- Kostnader för program varu prenumeration som SQL Database eller SUSE Linux-programvara ingår inte i Azures reservations priser

- Microsofts kommersiella priser till dig omfattar inte skatter, om inte din plats är Brasilien. Om din plats är Brasilien, är det kommersiella priset till dig att inkludera lämpliga skatter

- Försäljnings-och support agenter behöver uttrycklig åtkomst till Azure-prenumerationen så att de kan köpa eller hantera dem i Azure Portal-och fil support begär Anden, inklusive för utbyte och åter betalningar, för kundens räkning  

- Om du är en indirekt leverantör och du köper Azure-reservationer via Azure Portal, ärvs partnern av posten (indirekt åter försäljare) från den Azure CSP-prenumeration som du väljer.

- Det går inte att ändra partner till post för Azure-reservationer efter köp. Du kan avbryta den befintliga reservationen och köpa en ny med en ny partner av posten.

- Om en kund vill överföra en Azure-prenumeration från Direct eller EA till CSP, överförs inte reservationer.

## <a name="azure-reservations-unavailable-markets"></a>Azure-reservationer ej tillgängliga marknader

> [!IMPORTANT]
> Azure-reservationer **är inte** tillgängliga på följande marknader:  
>  
> **Ej tillgängliga marknader (i alfabetisk ordning)**
>
> |A till GI   | Gr till PAL  | PAP till Z |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | Åland     | Grönland     | Papua Nya Guinea     |
> | Amerikanska Samoa     | Grenada     | Pitcairn     |
> | Andorra     | Guadeloupe     | Réunion     |
> | Anguilla     | Guam     | Saba   |
> | Antarktis     | Guernsey     | Sankt Barthélemy   |
> | Antigua och Barbuda       | Guinea     | Saint Lucia   |
> | Aruba       | Guinea-Bissau     | Saint Martin   |
> | Azerbajdzjan       | Guyana     | Saint Pierre och Miquelon   |
> | Benin     | Haiti       | Saint Vincent och Grenadinerna     |
> | Bhutan     | Heard-och McDonaldöarna       | Samoa     |
> | Bonaire     | Isle of Man     | San Marino     |
> | Bouvetön     | Jan Mayen     | São Tomé och Príncipe   |
> | Brittiska territoriet i Indiska Oceanen       | Jersey     | Seychellerna   |
> | Brittiska Jungfruöarna     | Kiribati       | Sierra Leone   |
> | Burkina Faso     | Kosovo     | Sint Eustatius     |
> | Burundi     | Laos     | Sint Maarten     |
> | Kambodja     | Lesotho     | Solomonöarna     |
> | Centralafrikanska Republiken     | Liberia     | Somalia     |
> | Tchad     | Madagaskar     | Södra Georgien och Sydsandwichöarna     |
> | Kina     | Malawi     | Sydsudan     |
> | Julön     | Maldiverna     | Saint Helena, Ascension, Tristan da Cunha     |
> | Kokosöarna     | Mali     | Surinam     |
> | Komorerna     | Marshallöarna     | Svalbard     |
> | Kongo     | Martinique     | Swaziland     |
> | Kongo (DR)     | Mauretanien     | Timor-Leste   |
> | Cooköarna     | Mayotte     | Togo   |
> | Djibouti     | Mikronesien     | Tokelau   |
> | Dominica     | Montserrat     | Tonga   |
> | Ekvatorialguinea     | Moçambique     | Turks- och Caicosöarna   |
> | Eritrea     | Myanmar     | Tuvalu   |
> | Falklandsöarna     | Nauru     | USA:s yttre öar   |
> | Franska Guyana     | Nya Kaledonien     | Vanuatu   |
> | Franska Polynesien     | Niger     | Vatikanstaten   |
> | Franska sydterritorierna     | Niue     | Wallis och Futuna   |
> | Gabon     | Norfolkön     | Jemen   |
> | Gambia     | Nordmarianerna     |    |
> | Gibraltar     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Köp Azure-reservationer

Följ stegen nedan för att köpa Microsoft Azure reservationer för dina kunders räkning i Partner Center. (Vill du att kunderna ska kunna köpa sina egna Azure-reservationer från en tidigare Azure-prenumeration som du har köpt för dem? Se [ge kunderna tillstånd att köpa sina egna Azure-reservationer](give-customers-permission.md).)

1. Välj **kunder** från menyn Partner Center.  

2. På sidan **kunder** letar du reda på kunden som vill köpa Azure-reservationer och väljer sedan nedpilen för att expandera kundens rad.  

3. Välj **Lägg till produkter** och välj sedan **Azure**. 

    a. Välj kundens marknads segment i listan **segment** .

    b. Välj **reservationer** i listan produkt **typ** .

    c. Välj den typ av reservation som kunden vill ha från listan **reservations typ** .

4. Azure-reservationer måste associeras med en aktiv Azure-prenumeration. Välj den kund prenumeration som du vill lägga till Azure-reservationer i från listan med **kund prenumerationer** . 

   >[!IMPORTANT]
   >Om kunden inte redan har en aktiv Azure-prenumeration väljer du **Azure** för att lägga till en nu. 

5. Använd filtren för att hitta Azure-reservationer på virtuella datorer som uppfyller kundens krav.  

6. När du har hittat de reservationer som du vill köpa anger du det antal reserverade instanser som kunden behöver i **kvantitet** och väljer sedan **Lägg till i kundvagn**.  

7. Upprepa steg 5 och 6 tills du har lagt till alla nödvändiga objekt i ordern. Välj **Granska** för att kontrol lera att din beställning är korrekt.  

8. På sidan **Granska dina beställningar** kan du: 

    - Verifiera eller ändra antalet reserverade instanser.

    - Välj reservationens omfång. Reservationens omfång kan omfatta en prenumeration eller flera prenumerationer (delad omfattning). Om du omfångerar reservationen till en enskild prenumeration tillämpas reservations rabatten endast på den här prenumerationen. Om du väljer delad tillämpas reservations rabatten på alla prenumerationer i kundens fakturerings kontext. 

      >[!NOTE] 
      >Om du väljer att begränsa reservationens omfång till en enda Azure-prenumeration kan du behöva öka prenumerationens vCPU-kvot. Om du vill öka prenumerationens vCPU-kvot måste du skapa en support förfrågan i Azure Portal. Följ instruktionerna [i det här avsnittet](/azure/azure-supportability/resource-manager-core-quotas-request) för att skapa begäran. 

      >[!NOTE]   
      >Om din kund är under Azure-prenumerationen, ställs **scopet**  in på **delad**. 

    - Om du är en leverantörs partner väljer du den åter försäljare som du vill koppla till produkten.
    
    - Om din Azure-reservation stöder fakturerings Plans alternativet kan du välja fakturerings frekvensen som månatlig från List menyn. 
    - Om din Azure-reservation inte har stöd för fakturerings Plans alternativet är fakturerings frekvensen standardvärdet för en fakturerings tid. 

9. Välj **köp** för att köpa ordern. Informationen om din beställning, inklusive ditt beställnings nummer, visas på sidan **Bekräfta** . Välj **OK** för att gå till sidan **order historik** . 

10. Om du vill hantera kundens reservation i Azure Portal letar du upp kunden på sidan **kunder** och väljer sedan nedpilen för att expandera kundens rad. Välj **Microsoft Azure-hanteringsportal** för att öppna kundens post i Azure Portal.

## <a name="next-steps"></a>Nästa steg

|**För information om**   |**Läs detta**    |
|:-----------------------------|:-----------------|
|Översikt över Azure-reservationer i CSP  | [Sälj Microsoft Azure reserverade instanser](azure-reservations.md) |
|Hantera Azure-reservationer i Partner Center | [Hantera Azure-reservationer i Partner Center](azure-reservations-manage.md)
|Fastställ rätt storlek på virtuell dator och kontrol lera användningen av kund-VM   |[Storlek på virtuell dator för maximal användning av Azure-reservationer](azure-usage.md)   |
|Köpa Azure-reservationer med partner Center API | [Köp Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) i dokumentationen för partner Center-utvecklare   |
|Ge kunderna tillstånd att köpa sina egna Azure-reservationer  | [Ge kunderna tillstånd att köpa sina egna Azure-reservationer](give-customers-permission.md)  |