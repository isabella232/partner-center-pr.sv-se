---
title: Analysera prenumerationer och licenser
description: Lär dig hur du använder måtten på sidan prenumerations-och licens analys för att identifiera dina framgångar och områden som behöver mer uppmärksamhet.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.topic: article
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 03/31/2021
ms.openlocfilehash: 3f84026cc6402bea71837b06a5e330f2c879a06b
ms.sourcegitcommit: 766b2bb46dffd29e532b42106359f83e51b96700
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/31/2021
ms.locfileid: "106103799"
---
# <a name="analyze-subscriptions-and-licenses-to-help-you-drive-business-decisions-and-new-goals"></a>Analysera prenumerationer och licenser för att hjälpa dig att köra affärs beslut och nya mål

**Lämpliga roller**

- Global administratör
- Administratör för användar hantering
- Administratörs agent
- Försäljnings agent

Data enheter affärs beslut. Använd måtten på sidan **prenumerations-och licens analys** för att identifiera dina framgångar och områden som behöver mer uppmärksamhet. Använd den här informationen när du planerar nya affärs mål.

**TTM intäkt för CSP (USD)**: det här måttet representerar den sammanlagda summan av CSP-fakturerade intäkter (USD) för de efterföljande 12 månaderna (TTM) för de partner plats konton och globala partner kontot (pga) som detta CSP-konto är associerat med. Om du har andra CSP-konton med en annan PGA måste du logga in till var och en av dem för att kunna visa motsvarande aggregerade TTM-intäkter.  Klicka på länken Hämta information för att få en uppdelning av TTM-intäkterna per MPN-ID.

>[!NOTE]
>Lokala valuta priser (äldre Commerce FX) i kommersiellt läge hanteras i +/-5% av amerikanska dollar. Den äldre Commerce Exchange Rate (FX) skiljer sig från debiterings FX-priser som används av Azure i den moderna Commerce-upplevelsen. Taxan för modern Commerce-fakturerings FX baseras på Microsoft P&L-priser (Reuters FX-priser från stats matningar). Äldre priser för Commerce FX är Microsoft-konfidentiella.


Resten av rapporten kan pivotera utifrån följande produkter:

 - **Dynamics 365**: Dynamics 365-data  
 - **EMS**: Enterprise Management Services-data  
 - **Microsoft 365**: Microsoft 365 data  
 - **Office 365**: Office 365-data  


## <a name="types-of-subscription-and-license-metrics-you-can-view"></a>Typer av prenumerationer och licens mått som du kan visa

Vi spårar följande mått:

**Sammanfattning**  
 - **Sålda prenumerationer**: antal prenumerationer som skapats under den angivna tids perioden  
  
 - **Sålda licenser**: antal licenser som har sålts under den angivna tids perioden  
  
 - **Prenumerationer som förnyas på 30 dagar**: antal prenumerationer där statusen är aktiv under den angivna tids perioden och där **autoförnyelse** är sant
 
 - **Aktiva prenumerationer**: prenumerationer där status är **aktiv**  
 
 - **Pausade prenumerationer**: antal inaktiverade prenumerationer, det finns inget datum filter  

**Produkt analys**
  
 - **Antal prenumerationer**: de 5 främsta produkterna sorteras efter prenumerationer som sålts  
 
 - **Licens antal**: 5 främsta produkter efter sorterade licenser som säljs

**Kvarhållning av prenumeration**

 - **Förnyade prenumerationer**: prenumerationer som förnyas under de senaste 30 dagarna  

**Prenumerations omsättning**  
 - **Nya prenumerationer**: antal nya prenumerationer för tids perioden, förutom utvärderings erbjudanden  
 
 - **Avetablerade prenumerationer**: antal avetablerade eller inaktiverade prenumerationer efter datum  

**Inaktiverade prenumerationer** 
 
 - Lista över alla prenumerationer med statusen **pausad**, exklusive utvärderings erbjudanden  
  
**Aktiva prenumerationer**

 - Lista över alla aktiva prenumerationer  

**Konverteringar av utvärderings prenumeration**  

 - **Utvärderings version**: antal **aktiva** prenumerationer där utvärderings versionen betalar till konverteringen inträffade under den angivna tids perioden  

**Utvärderings prenumerationer som slutar på 30 dagar**  

 - Lista över försök som startades, där slutdatum ligger inom 30 dagar, och det inte finns något betalt start datum för prenumerationen  



## <a name="next-steps"></a>Nästa steg

- [Analysera prestanda för dina indirekta åter försäljare](analyze-indirect-resellers.md)