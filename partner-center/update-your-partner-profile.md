---
title: Verifiera företagets profil
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du verifierar företagets information, till exempel information om primär kontakt, adress och program. Du kan också uppdatera dina juridiska och fakturerings adresser.
author: parthpandyaMSFT
ms.author: parthp
ms.topic: how-to
ms.date: 03/10/2021
ms.localizationpriority: medium
ms.custom: contperf-fy21q3
ms.openlocfilehash: 5ade6d7c587561cc1af4a7645d1e4b0cce9a505e
ms.sourcegitcommit: 26095af7950817099764bf47370cb3e77e0dce7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "102770251"
---
# <a name="verify-or-update-your-company-profile-information"></a>Verifiera eller uppdatera företagets profil information 

**Lämpliga roller**

- Global administratör
- MPN-konto administratör

Första gången du loggar in på Partner Center som global administratör bör du kontrol lera att all företags information är korrekt. Detta omfattar primär kontakt, juridiskt företags namn, adress och programinformation. Om ditt företag har fler än en plats granskar du dina plats data för att se om det är korrekt. Som global administratör, fakturerings administratör eller administratörs agent kan du också se och uppdatera din fakturerings-och skatte information.

Din partner profil består av din juridiska företags information, det primära kontakt namnet och e-postmeddelandet, de program som företaget deltar i och, om så är tillämpligt, dina andra företag som nu är sammanslagna under din juridiska verksamhet. Kontrol lera att företags namnet och adressen i din juridiska affärs profil är fria från stavfel och att de matchar dina formella företags registrerings poster exakt. Om du arbetar som en enda ägare måste du använda ditt företags namn som juridiskt namn.


## <a name="locate-the-legal-business-profile"></a>Leta upp den juridiska företags profilen

1. Gå till **inställnings** ikonen och välj **konto inställningar**.
 
1. Välj **organisations profil**. 

2. Granska din **juridiska företags profil**, **primär kontakt information** och **programinformation**.

Om du har sammanfogat andra företag under din juridiska verksamhet kan du även granska informationen. 

## <a name="update-your-legal-business-profile"></a>Uppdatera din juridiska företags profil 

Uppdatera ditt juridiska företags namn eller din adress i Partner Center.

>[!Important]
>- För MPN-konton kan både den globala administratören och konto administratören uppdatera det juridiska företags namnet.
>- För konton med indirekt åter försäljare av CSP kan bara den globala administratören uppdatera det juridiska företags namnet. 
>- Direkt fakturerings partner och indirekta leverantörer kan inte ändra det juridiska namnet på företaget om konto verifierings statusen är **auktoriserad**. Om du behöver ändra namnet måste du skapa ett [support ärende](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=eb74583c-61b3-2124-bffc-00920e0ae772).



1. Gå till **Inställningar**, **konto inställningar** och välj **organisations profil**.

2. Välj **juridisk**  information och välj sedan den juridiska företags profil (partner eller åter försäljare) som du vill uppdatera.

1. Klicka på **Uppdatera**  bredvid företags namn/adress och ändra informationen.
 
1. När du väljer **Skicka**, kommer din juridiska identitet att utvärderas igen.

1. Om verifieringen Miss lyckas kan du läsa om hur du [åtgärdar problemet](verification-responses.md).

>[!Important]
>Om du är en partner av en moln lösnings leverantör kan du inte ändra det land som är associerat med din juridiska adress. Ditt juridiska adress land är knutet till din klient och dina tjänster samt den valuta som du gör affärer med. Mer information om MPN finns i  [land uppdateringar för MPN](manage-locations.md#change-country-of-partner-global-account).


### <a name="who-can-update-legal-business-name-and-when"></a>Vem kan uppdatera juridisk företags namn och när

|**Program**|**Vem kan uppdatera företags namn**|**När (status) kan uppdateras**|**Tillåts**|
|---------------------|:-------------------------------|:------------|:-----------------|
MPN|Global administratör; Konto administratör|Auktorisation väntande slagit| Tillåts|
|CSP: indirekt åter försäljare|Global administratör|Auktorisation väntande slagit| Tillåts|


## <a name="update-your-mpn-global-business-account"></a>Uppdatera ditt MPN globala företags konto

Om fel företags kontot under migreringen från partner medlemskaps Center till Partner Center har identifierats som juridiskt företag, kan du ändra det till rätt juridiskt företags konto.

Om du vill göra dessa uppdateringar måste du vara antingen den globala administratören eller konto administratören. Lär dig hur du [hanterar dina MPN globala plats konton](manage-locations.md)


## <a name="update-your-mpn-id-associated-with-your-csp-account"></a>Uppdatera MPN-ID:t som är associerat med ditt CSP-konto

Så här uppdaterar du det MPN-ID som är associerat med ditt CSP-konto:

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard/home) för partner Center som global administratör med dina AUTENTISERINGSUPPGIFTER för CSP-kontot och välj sedan **Inställningar**. (Dina autentiseringsuppgifter för MPN och CSP kan vara olika.)
 
1. Välj **identifierare** från **konto inställningar**.

1. Under avsnittet **CSP** använder du länken **Uppdatera** för att uppdatera det MPN-ID som är associerat med ditt CSP-konto 


## <a name="update-your-csp-legal-billing-address"></a>Uppdatera din CSP-juridiska fakturerings adress

Om du är global administratör, fakturerings administratör eller administratörs agent kan du ändra adressen som visas på fakturan i din **utbetalnings-och skatte profil**. Du kan dock inte ändra företagsnamnet på fakturan på grund av en begränsning i fakturasystemet.


## <a name="next-steps"></a>Nästa steg

- [Kontrol lera verifierings status](verification-responses.md)

- [Hantera MPN-platser](manage-locations.md)
