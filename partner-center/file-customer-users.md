---
title: Fält för .csv för att importera flera användare för ett kundkonto
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Om du vill lägga till flera användare till ett kundkonto skapar du en fil med kommaavgränsade värden (.csv) med lämpliga fält.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d8cbeecf081dc82448625daeedc0ce21b31174e
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114838350"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Lägga till flera användare till ett kundkonto genom att skapa .csv fil

**Lämpliga roller:** Global administratör

Lägg till flera användare till en kunds konto samtidigt genom att ladda upp en datafil i filformatet med kommaavgränsade värden (.csv) till Partnercenter. Du kan ladda ned en exempeldatafil från Partnercenter och sedan redigera den för din användning, eller så kan du skapa en ny datafil med hjälp av den datamodell som definieras nedan.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Krav för datafiler

Om du vill lägga till flera användare till en kunds konto med massuppladdningsprocessen måste du uppfylla följande krav:

- Du måste ha behörighet som global administratör för kundkontot.
- Varje användare måste ha en unik e-postadress som läggs till i kundens e-postdomäner;
- Du kan ladda upp upp till 100 poster i taget. Om du behöver lägga till fler än 100 användare kan du skapa och ladda upp ytterligare datafiler.
- Alla användare måste finnas på samma geografiska **plats.**
- Ange endast de data som beskrivs nedan. Överflödiga data gör att uppladdningen misslyckas.

Ange följande data i datafilen:

| **Kolumnnamn** | **Beskrivning**  | **Begränsning**  |
|:-------- |:------  |:----- |
| Förnamn  | Användarens förnamn (valfritt fält)  | Gräns på 50 tecken  |
| Efternamn  | Användarens efternamn (valfritt fält)  | Gräns på 50 tecken  |
| Visningsnamn    | Namn som visas i Partnercenter (obligatoriskt fält)                            | Gräns på 50 tecken                         |
| E-post   | Användarens företags-e-postadress på kundföretaget (obligatoriskt fält)           | Varje användare måste ha en unik e-postadress |
| Statusuppdatering   | Används för att ange om den nya användarposten har skapats | \*\*Lämna tomt\*\*                        |

## <a name="next-steps"></a>Nästa steg

- [Så här lägger du till flera användare för en kund](adding-multiple-users-to-a-customer-account.md)