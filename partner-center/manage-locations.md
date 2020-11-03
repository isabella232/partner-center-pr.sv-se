---
title: Hantera platser i ditt partner konto
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur du lägger till en ny plats och hur plats MPN ID används i stimulans program, CSP-verksamhet, prenumerationer och andra transaktioner.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c6b0fc84636befedbc51aa0672ce19110eb4d9aa
ms.sourcegitcommit: 1719ff11409cd6953602b7798f8cfe821b8ea15e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/15/2020
ms.locfileid: "92531972"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Hantera dina MPN-konto platser och Lägg till en ny plats

**Gäller för**

- Partnercenter

**Lämpliga roller**

- Global administratör
- Kontoadministratör

Platsens MPN-ID identifierar varje enskild plats för ditt företag. Du kan använda platsens MPN-ID för att registrera dig för stimulans program, till Transact Cloud Solution Provider (CSP) Business och andra affärs transaktioner. Det globala MPN-ID: t används för icke-transaktionella aktiviteter, till exempel support förfrågningar.

## <a name="the-following-is-a-typical-scenario"></a>Följande är ett typiskt scenario:

Contoso har sitt globala partner konto (PGA) i Storbritannien. Detta är deras registrerade juridiska verksamhet och det globala MPN-ID används för att hantera all icke-transaktionell verksamhet. Contoso har även ett konto för partner lokalisering (PLA) som motsvarar dotter bolag eller divisioner på en annan plats i Storbritannien, Frankrike och USA. I MPN-konto strukturen visas dessa PLAs som unika plats MPN-ID: n. PLAs används för transaktions företag som CSP eller incitaments program. Utbetalningar är knutna till vissa platser. 

>[!NOTE]
>Det finns en 1-1-relation mellan en CSP-klient och en MPN plats-ID.

:::image type="content" source="images/locations/locations1.png" alt-text="Struktur för MPN-platser":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>Krav för att lägga till en ny plats för en CSP-verksamhet

För att lägga till en ny KRYPTOGRAFIPROVIDERs affärs plats finns det flera krav:

1. Du måste ha ett plats MPN-ID i det land där du vill göra affärer.

1. Du behöver en ny Azure AD-klient i [affärs området](regional-authorization-overview.md) som inte redan har registrerats i CSP. Skapa det när du registrerar i CSP.
 
3. Använd den nya AAD-klienten för att registrera i CSP-programmet i regionen.
Ange juridisk information om företaget, inklusive juridisk företags namn, adress, primär kontakt information. Det här kontot kommer att genomgå verifiering, så se till att lägga till giltig information.

>[!NOTE] 
 >Kom ihåg att logga in med de **nya** autentiseringsuppgifterna för den **nya** Azure AD-klienten. Använd inte dina befintliga autentiseringsuppgifter eftersom Partner Center känner igen att du redan har ett konto.

4. Godkänn Microsoft partner Agreement och aktivera kontot.

## <a name="add-an-mpn-location"></a>Lägg till en MPN-plats

1. Logga in med MPN-kontot i Partner Center. MPN-kontot ska ha global administratör eller konto administratörs behörighet. 

1. I **inställnings ikonen** väljer du **partner inställningar** .

2. Välj **platser.**

3. Välj **Lägg till en plats** och Infoga adress information för den plats som du vill lägga till i företaget samt en primär kontakt för platsen.

> [!NOTE]
> Det går inte att ta bort en plats som har lagts till i Partner Center. Du kommer att se **MPN** på den vänstra menyn i Partner Center om du har använt rätt MPN-ID för att logga in.

## <a name="change-global-partner-account-location"></a>Ändra plats för global partner konto

1. På sidan **[platser](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** kontrollerar du listan över platser för att se till att den plats som du vill använda som juridisk person visas. Om den inte är det lägger du till den.

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Struktur för MPN-platser":::

2. Välj **partner profil** och välj sedan **Uppdatera juridisk företags profil**

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Struktur för MPN-platser":::

3. Välj region och juridisk person och **Skicka** den.

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Struktur för MPN-platser":::

## <a name="next-steps"></a>Nästa steg

- Lär dig mer om [verifierings processen](verification-responses.md).
