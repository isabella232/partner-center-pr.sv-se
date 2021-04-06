---
title: Hantera platser i ditt partner konto
ms.topic: how-to
ms.date: 04/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur du lägger till en ny plats och hur plats MPN ID används i stimulans program, CSP-verksamhet, prenumerationer och andra transaktioner.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ca8c866479fbe153c1e0192edd33e8258b9d6e7
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441343"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Hantera dina MPN-konto platser och lägga till (ta bort) en plats


**Lämpliga roller**

- Global administratör
- Kontoadministratör

Platsens MPN-ID identifierar varje enskild plats för ditt företag. Du kan använda platsens MPN-ID för att registrera dig för stimulans program, till Transact Cloud Solution Provider (CSP) Business och andra affärs transaktioner. Det globala MPN-ID: t används för icke-transaktionella aktiviteter, till exempel support förfrågningar.

## <a name="the-following-scenario-is-typical"></a>Följande scenario är vanligt:

Contoso har sitt globala partner konto (PGA) i Storbritannien. PGA är sitt registrerade juridiska företag och det globala MPN-ID: t används för att hantera all icke-transaktionell verksamhet. Contoso har även ett konto för partner lokalisering (PLA) som motsvarar dotter bolag eller divisioner på en annan plats i Storbritannien, Frankrike och USA. I MPN-konto strukturen visas dessa PLAs som unika plats MPN-ID: n. PLAs används för transaktions företag som CSP eller incitaments program. Utbetalningar är knutna till vissa platser. 

>[!NOTE]
>Det finns en 1-1-relation mellan en CSP-klient och en MPN plats-ID.

:::image type="content" source="images/locations/locations1.png" alt-text="Struktur för MPN-platser":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Krav för att lägga till ett nytt konto för en CSP-verksamhet

Om du vill lägga till ett nytt CSP-affärskonto börjar du med att se till att du uppfyller kraven.

1. Du måste ha ett plats MPN-ID i det land där du vill göra CSP-verksamhet. Om du vill skapa en ny MPN plats läser du "Lägg till en MPN plats" nedan.
  
1. Om du vill skapa en ny CSP indirekt åter försäljares registrering, Läs [arbeta med indirekta leverantörer](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Kom ihåg att logga in med de **nya** autentiseringsuppgifterna för det **nya** CSP-kontot. Använd inte dina befintliga autentiseringsuppgifter eftersom Partner Center känner igen att du redan har ett konto.

2. Godkänn Microsoft partner Agreement och aktivera kontot.

1. Läs [krav för direkt fakturerings](direct-partner-new-requirements.md) partner om du vill registrera dig som en direkt fakturerings partner

## <a name="view-your-mpn-locations"></a>Visa dina MPN-platser

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard/home) för partner Center med dina MPN-kontoautentiseringsuppgifter. (Dina MPN-autentiseringsuppgifter kan skilja sig från dina autentiseringsuppgifter för CSP) 
 
1. I **inställnings** ikonen väljer du **konto inställningar**, **organisations profil**, **Legal**. 

1. På fliken **partner** kontrollerar du att det inte finns ett informations fel meddelande som ber dig att åtgärda migrerade platser från PMC.  Om dina platser inte har ställts in korrekt i PMC och inte har övergått till dator än PC måste du uppdatera dessa platser.

:::image type="content" source="images/locations/location-two.png" alt-text="Skärm bild visar hur du uppdaterar platsen.":::
 
4.  På skärmen **Granska PMC-platser** väljer du **Uppdatera**.
Uppdatera följande fält:

- **Namnfält**: kontrol lera att namnet på företags platsen är korrekt. Om ett duplicerat fel visas kan du försöka ändra från, till exempel contoso till contoso, Inc.

- **Fält för juridisk person**: kontrol lera att du har valt den juridiska personen som platsen är kopplad till

- **Adress rad 1 & 2 fält**: kontrol lera att adressen är korrekt

- **Fälten ort & delstat/provins**: se till att kombinationen mellan staden och regionen är korrekt. Det finns länder där List menyn för att välja delstat/provins ska tillämpas och i andra länder måste fältet infogas manuellt.

- **Fält för post** nummer: kontrol lera att post nummer fältet matchar ditt angivna land, region, ort eller adress.

- **Fält för primär kontakt information**: se till att fälten för första och sista namn är fyllda och att den angivna e-postadressen är en e-postadress för arbetet och inte en personlig (t @outlook.com . ex., @live.com osv.)

- **Telefonnummer fält**: kontrol lera att telefonnumret inte innehåller specialtecken, mellanslag eller landskod. Värdet som anges i fältet telefonnummer får alltid innehålla högst 10 tecken.

5. Om det inte finns något fel meddelande väljer du **konto inställningar**, **organisations profil** och **identifierare** i **Inställningar**.

6. Hitta MPN-ID: t med typen "location" som matchar landet för det här CSP-kontot och Använd det för att slutföra associationen.

7. Om du inte hittar platsens MPN-ID som matchar det CSP-konto som du vill använda, kan du lägga till en ny plats, vilket skapar ett nytt MPN-ID. Se **lägga till en MPN plats** nedan.

## <a name="add-an-mpn-location"></a>Lägg till en MPN-plats

1. Logga in med MPN-kontot i Partner Center. (Dina MPN-autentiseringsuppgifter kan skilja sig från dina autentiseringsuppgifter för din CSP). MPN-kontot ska ha global administratör eller konto administratörs behörighet. 

1. Från **inställnings ikonen** väljer du **konto inställningarna** och väljer sedan **organisations profil**.

2. Välj **juridiskt** och sedan på fliken **partner** väljer du **företags platser** och klickar på **Lägg till en plats.**

3. Ange nödvändig information, inklusive företags namn, adress och kontakt för den plats som du vill lägga till i företaget.
 
1. Klicka på **Lägg till plats**. Då skapas ett nytt MPN-ID för den nya platsen som du kan använda för CSP-transaktioner och-incitament.

:::image type="content" source="images/legal-biz.png" alt-text="Lägg till en ny juridisk verksamhet":::

> [!NOTE]
> När en plats har lagts till i Partner Center kan du inte ta bort den. Du kommer att se **MPN** på den vänstra menyn i Partner Center om du har använt rätt MPN-ID för att logga in.


## <a name="delete-a-location"></a>Ta bort en plats

Om du vill ta bort en plats från ditt konto måste du kontakta [partner support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b). Se till att du förstår den påverkan den här åtgärden har. Det går inte att hämta borttagna platser och något som är knutet till det aktuella MPN-ID: t kan inte längre identifieras eller vara aktivt för ditt företag.

## <a name="change-country-of-partner-global-account"></a>Ändra land för globalt partner konto 

1. Logga in med MPN-kontot i Partner Center. (Dina MPN-autentiseringsuppgifter kan skilja sig från dina autentiseringsuppgifter för din CSP). MPN-kontot ska ha global administratör eller konto administratörs behörighet. 

2. På fliken **partner** går du till **företags platser** och kontrollerar listan över platser för att se till att den plats som du vill använda som juridisk person visas. 
 
1. Om du vill lägga till en plats klickar du på **Lägg till en plats** och anger den information som krävs, till exempel företags namn, adress och primär kontakt för den plats som du vill lägga till i företaget. 
 
1. Välj **ändra ditt land** bredvid List rutan **land/region** och följ stegen. 

:::image type="content" source="images/lbp.png" alt-text="Information om juridisk företags profil, flyg ut":::

5. Klicka på **Spara**.

6. MPN globalt konto land kommer att ändras till det nya juridiska landet.
  
## <a name="next-steps"></a>Nästa steg

- Lär dig mer om [verifierings processen](verification-responses.md).
