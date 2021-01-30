---
title: Hantera platser i ditt partner konto
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur du lägger till en ny plats och hur plats MPN ID används i stimulans program, CSP-verksamhet, prenumerationer och andra transaktioner.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21d82fc3ec4470d4941d3ca7436089d3e892439e
ms.sourcegitcommit: 81017727107a907bf1f3246097b51667d7c5fb18
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/30/2021
ms.locfileid: "99098898"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Hantera dina MPN-konto platser och Lägg till en ny plats


**Lämpliga roller**

- Global administratör
- Kontoadministratör

Platsens MPN-ID identifierar varje enskild plats för ditt företag. Du kan använda platsens MPN-ID för att registrera dig för stimulans program, till Transact Cloud Solution Provider (CSP) Business och andra affärs transaktioner. Det globala MPN-ID: t används för icke-transaktionella aktiviteter, till exempel support förfrågningar.

## <a name="the-following-is-a-typical-scenario"></a>Följande är ett typiskt scenario:

Contoso har sitt globala partner konto (PGA) i Storbritannien. Detta är deras registrerade juridiska verksamhet och det globala MPN-ID används för att hantera all icke-transaktionell verksamhet. Contoso har även ett konto för partner lokalisering (PLA) som motsvarar dotter bolag eller divisioner på en annan plats i Storbritannien, Frankrike och USA. I MPN-konto strukturen visas dessa PLAs som unika plats MPN-ID: n. PLAs används för transaktions företag som CSP eller incitaments program. Utbetalningar är knutna till vissa platser. 

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

## <a name="view-your-mpn-locations"></a>Visa dina MPN-platser

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard/home) för partner Center med dina MPN-kontoautentiseringsuppgifter. (Dina MPN-autentiseringsuppgifter kan skilja sig från dina autentiseringsuppgifter för CSP) 
 
1. I **inställnings** ikonen väljer du **konto inställningar**, **organisations profil**, **Legal**. 

1. På fliken **partner** kontrollerar du att det inte finns något informations fel meddelande som ber dig att åtgärda migrerade platser från PMC. Följ anvisningarna och åtgärda dessa platser. 

3. Om det inte finns något fel meddelande väljer du **konto inställningar**, **organisations profil** och **identifierare** i **Inställningar**.

4. Hitta MPN-ID: t med typen "location" som stämmer överens med det här CSP-kontots land och Använd det för att söka efter och slutföra associationen.

5. Om du inte hittar platsens MPN-ID som matchar det CSP-konto som du vill använda, kan du lägga till en ny plats som skapar ett nytt MPN-ID. Se **lägga till en MPN plats** nedan.

## <a name="add-an-mpn-location"></a>Lägg till en MPN-plats

1. Logga in med MPN-kontot i Partner Center. (Dina MPN-autentiseringsuppgifter kan skilja sig från dina autentiseringsuppgifter för din CSP). MPN-kontot ska ha global administratör eller konto administratörs behörighet. 

1. Från **inställnings ikonen** väljer du **konto inställningarna** och väljer sedan **organisations profil**.

2. Välj **juridiskt** och sedan på fliken **partner** väljer du **företags platser** och klickar på **Lägg till en plats.**

3. Ange nödvändig information, inklusive företags namn, adress och kontakt för den plats som du vill lägga till i företaget.
 
1. Klicka på **Lägg till plats**. Då skapas ett nytt MPN-ID för den nya platsen som du kan använda för CSP-transaktioner och-incitament.

:::image type="content" source="images/legal-biz.png" alt-text="Lägg till en ny juridisk verksamhet":::

> [!NOTE]
> Det går inte att ta bort en plats som har lagts till i Partner Center. Du kommer att se **MPN** på den vänstra menyn i Partner Center om du har använt rätt MPN-ID för att logga in.

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
