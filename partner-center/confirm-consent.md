---
title: Bekräfta kund godkännande av Microsofts kund avtal
description: Lär dig hur du bekräftar kund godkännande av Microsofts kund avtal. Det kan vara nödvändigt att beställa Microsoft-produkter och-tjänster för kunder.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: aacca72e9af45b2777364734c2b07dbe8101989d
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532124"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Uppdaterad metod för att bekräfta kund godkännande av Microsofts kund avtal

**Gäller för**

-  Partnercenter

**Lämpliga roller**

- Administratörs agent
- Försäljnings agent

> [!NOTE]
> Avtals resursen stöds för närvarande av Partner Center i det offentliga Microsoft-molnet. Det gäller inte för:
> * Partner Center som drivs av 21Vianet
> * Partner Center för Microsoft Cloud Germany
> * Partner Center för Microsoft Cloud för amerikanska myndigheter

>[!NOTE]
>Från och med den 31 januari 2020 måste alla kunder, befintliga och nya, signera det nya Microsofts kund avtal. Läs mer i [bekräfta kund godkännande av Microsofts kund avtal](confirm-customer-agreement.md).

Som partner måste du inhämta kundens godkännande av Microsofts kund avtal innan du kan beställa Microsofts produkter och tjänster för kunden. För att bättre hjälpa partners att uppfylla kraven för efterlevnad ber Microsoft partners att bekräfta godkännande genom att tillhandahålla följande information om den person som har godkänt avtalet:

- Förnamn

- Efternamn

- E-postadress

- Telefonnummer (valfritt)

- Datum för godkännande

Direkta fakturerings partner och indirekta leverantörer måste bekräfta kund godkännande av Microsofts kund avtal vid kommunikation via partner Center eller API för partner Center. Bekräftelse är *obligatorisk* .

Om ingen bekräftelse anges för en angiven kund:

- Du kommer inte att kunna skapa nya beställningar för den här kunden.

- Du kommer inte att kunna ändra licens antalet för befintliga licensbaserade prenumerationer för den här kunden.

Bekräftelse av kund godkännande kan göras via partner Center eller partner Center API. Om du vill göra detta via partner Center API, se följande avsnitt:

- [Få bekräftelse på kund medgivande](/partner-center/develop/get-confirmation-of-customer-consent)

- [Hämta avtals metadata](/partner-center/develop/get-agreement-metadata)

- [Bekräfta kund medgivande](/partner-center/develop/confirm-customer-consent)

Detta gäller för både produktions-och sandbox-miljöer.

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>Bekräfta kund godkännande för en ny kund

Använd följande procedur för att bekräfta kund godkännande när du skapar en ny kund klient i Partner Center. Du måste vara administratörs agent eller försäljnings agent för att göra detta.

1. Välj **kunder** och sedan **ny kund** och välj sedan **konto information** .

2. Ange information om **företaget** och den **primära kontakten** .

   :::image type="content" source="images/mca/mca1.png" alt-text="Företags information":::

3. Under **Microsofts kund avtal** väljer **du kunden har accepterat det senaste kund avtalet från Microsoft** .

4. Ange ett datum under **avtalets godkännande datum** . Du kan inte ange ett framtida datum.

5. Ange information om den användare som tillhandahöll godkännandet.

   :::image type="content" source="images/mca/MCA3.png" alt-text="Företags information":::

   Som standard visas den primära kontaktens användar information. Om detta inte är korrekt väljer du **Uppdatera** och anger sedan **förnamn** , **efter namn** , **e-postadress** och * *telefonnummer* (valfritt) för den person som har godkänt avtalet.

6. Välj **Nästa** för att fortsätta med de återstående stegen för att skapa kund klienten.

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Bekräfta kund godkännande för en befintlig kund

Du måste vara administratörs agent eller försäljnings agent för att göra detta.

1. Välj **kunder** och leta upp och välj den kund som du vill se.

2. Välj **konto information** .

3. Under **Microsofts kund avtal** väljer du **Uppdatera** .

   :::image type="content" source="images/mca/mca4.png" alt-text="Företags information":::

4. Ange **förnamn** , **efter namn** , **e-postadress** och **telefonnummer** (valfritt) för den användare som har godkänt avtalet.

5. Ange ett datum under **avtalets godkännande datum** . Du kan inte ange ett framtida datum.

6. Välj **Spara och fortsätt** .

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Bekräfta kund godkännande när du skapar en ny order för en befintlig kund

Om du försöker skapa en ny order för en befintlig kund som du inte har bekräftat tidigare får du ett meddelande om att slutföra bekräftelsen. Använd följande procedur för att göra detta.

1. Ange **förnamn** , **efter namn** , **e-postadress** och **telefonnummer** (valfritt) för den användare som har godkänt avtalet.

2. Ange ett datum under **avtalets godkännande datum** . Du kan inte ange ett framtida datum.

3. Välj **Spara och fortsätt** .

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Hämta bekräftelse av kund godkännande för en befintlig kund

Du kan hämta bekräftelse på kund godkännande för en befintlig kund som du har angett tidigare med hjälp av proceduren nedan. Du måste vara administratörs agent eller försäljnings agent för att göra detta.

1. Välj **kunder** och leta upp och välj den kund som du vill se.

2. Välj **konto information** .

3. Under **Microsofts kund avtal** ser du om en bekräftelse har angetts för kunden.

## <a name="next-steps"></a>Nästa steg

- [Bekräfta kund godkännande av Microsofts kund avtal i CSP partner-programmet](confirm-customer-agreement.md)

- [Attestering av godkännande av Microsofts kund avtal för kundens räkning](attest-acceptance-customer-agreement.md)