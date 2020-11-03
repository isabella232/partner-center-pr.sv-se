---
title: Fält för. csv-fil för att importera flera användare för ett kund konto
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Om du vill lägga till flera användare i ett kund konto skapar du en fil med kommaavgränsade värden (. csv) med lämpliga fält.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/03/2020
ms.locfileid: "92531160"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Lägg till flera användare till ett kund konto genom att skapa en. csv-fil

**Gäller för**

- Partnercenter

**Lämpliga roller**

- Global administratör

Lägg till flera användare till ett kund konto samtidigt, genom att ladda upp en datafil i det kommaavgränsade värde fil formatet (. csv) till Partner Center. Du kan ladda ned en exempel data fil från Partner Center och sedan redigera den för din användning, eller så kan du skapa en ny datafil med hjälp av den data modell som anges nedan.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Krav för data fil

Om du vill lägga till flera användare till ett kund konto med processen för Mass uppladdning måste du uppfylla följande krav:

- Du måste ha global administratörs behörighet till kund kontot.
- Varje användare måste ha en unik e-postadress som läggs till kundens e-postdomän.
- Du kan ladda upp upp till 100 poster i taget. Om du behöver lägga till fler än 100 användare skapar du och laddar upp ytterligare datafiler.
- Alla användare måste finnas på samma geografiska **plats** .
- Ange endast de data som beskrivs nedan. Främmande data gör att överföringen Miss fungerar.

Ange följande data i data filen:

| **Kolumnnamn** | **Beskrivning**  | **Begränsning**  |
|:-------- |:------  |:----- |
| Förnamn  | Användarens förnamn (valfritt fält)  | 50 – tecken gräns  |
| Efternamn  | Användarens efter namn (valfritt fält)  | 50 – tecken gräns  |
| Visningsnamn    | Namn som visas i Partner Center (obligatoriskt fält)                            | 50 – tecken gräns                         |
| E-post   | Användarens företags-e-postadress på kund företaget (obligatoriskt fält)           | Varje användare måste ha en unik e-postadress |
| Status uppdatering   | Används för att ange om den nya användar posten har skapats eller inte | \*\*Lämna tomt\*\*                        |

## <a name="next-steps"></a>Nästa steg

- [Så här lägger du till flera användare för en kund](adding-multiple-users-to-a-customer-account.md)