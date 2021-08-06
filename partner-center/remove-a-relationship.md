---
title: Ta bort återförsäljarrelation med en kund
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Ta reda på hur Microsofts direktpartner kan ta bort kunder från listan, ta bort delegerade administratörsbehörigheter och sluta stödja eller köpa för en kund.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 28f08cf1b15ccc944c8980b4111c583ccda948a35412ff0edb176a2e65f308df
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115678143"
---
# <a name="how-to-remove-a-reseller-relationship-with-a-customer-in-partner-center"></a>Så här tar du bort en återförsäljarrelation med en kund i Partnercenter

**Lämpliga roller:** Global administratör

Den här artikeln beskriver hur du tar bort en återförsäljarrelation med en kund i Partnercenter.

Direkta partner eller indirekta leverantörer: Om du inte längre handlar med en kund kan du ta bort relationen i Partnercenter.

Borttagning av en relation har följande konsekvenser:

- Kunden tas bort från din lista över kunder i Partnercenter
- Tar bort dig från [listan över tillgängliga supportkontakter](assign-support-contacts.md) för din kund
- Dina administratörsprivilegier för delegering för kunden tas bort
- Du kan inte göra framtida inköp för kunden

## <a name="how-to-remove-a-relationship"></a>Så här tar du bort en relation

Om du vill ta bort relationen måste du avbryta reservationer för reserverad Azure-instans (RI), avbryta programvaruinköp och inaktivera eventuella återstående aktiva prenumerationer först.

1. **Pausa alla aktiva prenumerationer.**

   1. Från Partnercenter går du till **Kunder** och väljer en kund

   2. Under **Prenumerationer** väljer du en prenumeration.

   3. Välj **Pausad**

   4. Upprepa dessa steg för varje aktiv prenumeration.

2. **Ta bort relationen i Partnercenter:**

   a. Från Partnercenter går du till **Kunder** och väljer en kund.

   b. Välj **Kontot**.

   c. Välj **Ta bort återförsäljarrelation.**

   > [!NOTE]
   > Om några prenumerationer fortfarande är aktiva kommer länken **Ta bort återförsäljarrelation** att vara inaktiv.

## <a name="next-steps"></a>Nästa steg

- [Begära eller återupprätta en relation med en kund](request-a-relationship-with-a-customer.md)
