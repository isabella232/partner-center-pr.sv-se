---
title: Hantera platser i ditt partnerkonto
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-membership
description: Lär dig hur du lägger till en ny plats och hur platsens MPN-ID används i incitamentprogram, CSP-företag, prenumerationer och andra transaktioner.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 66ca3a24a810f61eae9feece5e64440fa531cda5
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836990"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Hantera dina MPN-kontoplatser och lägg till (ta bort) en plats


**Lämpliga roller:** Global | Kontoadministratör

Platsens MPN-ID identifierar varje specifik plats för ditt företag. Du använder platsens MPN-ID för att registrera dig för incitamentprogram, för att Molnlösningsleverantör företag (CSP) och andra affärstransaktioner. Det globala MPN-ID:t används för icke-transaktionella aktiviteter, till exempel supportbegäranden.

## <a name="the-following-scenario-is-typical"></a>Följande scenario är typiskt:

Contoso har sitt globala partnerkonto (PGA) i Storbritannien. PGA är deras registrerade juridiska verksamhet och dess globala MPN-ID används för att hantera alla icke-transaktionella företag. Contoso har också partnerplatskonton (PLA) som motsvarar dotterbolag eller avdelningar på en annan plats i Storbritannien, Frankrike och USA. I MPN-kontostrukturen representeras dessa PLA:er som MPN-ID:er för unika platser. PLA:erna används för transaktionella företag, till exempel CSP eller incitamentsprogram. Utbetalningarna är knutna till specifika platser. 

>[!NOTE]
>Det finns en 1-1-relation mellan en CSP-klient och ett MPN-plats-ID.

:::image type="content" source="images/locations/locations1.png" alt-text="Strukturen för MPN-platser.":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Krav för att kunna lägga till ett nytt konto för en CSP-verksamhet

Om du vill lägga till ett nytt CSP-företagskonto börjar du med att se till att du uppfyller kraven.

1. Du måste ha ett PLATS-MPN-ID i det land där du vill göra CSP-verksamhet. Om du vill skapa en ny MPN-plats läser du "Lägg till en MPN-plats" nedan.
  
1. Om du vill skapa en CSP Indirect Reseller registrering kan du läsa [Arbeta med indirekta leverantörer](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Kom ihåg att logga in med de **nya autentiseringsuppgifterna** för det **nya** CSP-kontot. Använd inte dina befintliga autentiseringsuppgifter eftersom Partnercenter identifierar dig som att du redan har ett konto.

2. Godkänn Microsoft-partneravtal och aktivera kontot.

1. Om du vill registrera dig som direktfaktureringspartner läser du [Krav för direktfaktureringspartner](direct-partner-new-requirements.md)

## <a name="view-and-update-your-mpn-locations"></a>Visa och uppdatera DINA MPN-platser

1. Logga in på instrumentpanelen i [Partnercenter med](https://partner.microsoft.com/dashboard/home) dina MPN-kontoautentiseringsuppgifter. (Dina MPN-autentiseringsuppgifter kan vara annorlunda än dina CSP-autentiseringsuppgifter) 
 
1. Från ikonen **Inställningar** väljer du **Kontoinställningar**, **Organisationsprofil**, **Juridiskt**. 

1. På fliken **Partner** kontrollerar du att det inte finns något banderollsfelmeddelande där du uppmanas att åtgärda migrerade platser från PMC.  Om dina platser inte har ställts in korrekt i PMC och ännu inte har gått över till datorn måste du uppdatera dessa platser.

:::image type="content" source="images/locations/location-two.png" alt-text="Skärmbild som visar hur du uppdaterar platsen.":::
 
4.  På skärmen **Granska PMC-platser** väljer du **Uppdatera**.
Uppdatera följande fält:

- **Namnfält:** Kontrollera att namnet på företagets plats är korrekt. Om ett duplicerat fel visas kan du prova att byta från till exempel Contoso till Contoso, Inc.

- **Fältet Juridisk enhet:** Kontrollera att du har valt den juridiska enhet som platsen är kopplad till

- **Adressrad 1 & 2 fält:** Kontrollera att adressen är korrekt

- **Fält & stad/provins:** Kontrollera att kombinationen mellan staden och delstaten/provinsen är korrekt. Det finns länder där den nedrullningsbara menyn för att välja delstat/provins kommer att gälla, och i andra länder måste fältet infogas manuellt.

- **Postnummerfält:** Kontrollera att postnummerfältet matchar ditt angivna land, region, ort eller adress.

- **Fält med primär** kontaktinformation: Kontrollera att fälten för för- och efternamn är ifyllda och att e-postadressen som anges är en e-postadress för arbetet och inte en personlig e-postadress (till exempel @outlook.com , @live.com osv.)

- **Telefon:** Kontrollera att Telefon inte innehåller specialtecken, blanksteg eller landskod. Värdet som anges Telefon fältet Antal innehåller alltid högst 10 tecken.

5. Om det inte finns något felmeddelande går du till **Inställningar** väljer **Konto Inställningar,** **Organisationsprofil**, **Identifierare**.

6. Hitta MPN-ID:t med typen "Plats" som matchar landet för det här CSP-kontot och använd det för att slutföra associationen.

7. Om du inte hittar platsens MPN-ID som matchar det CSP-konto som du vill använda kan du lägga till en ny plats, vilket skapar ett nytt MPN-ID. Se **Lägg till en MPN-plats** nedan.

## <a name="add-an-mpn-location"></a>Lägga till en MPN-plats

1. Logga in med MPN-kontot i Partnercenter. (Dina MPN-autentiseringsuppgifter kan vara annorlunda än dina CSP-autentiseringsuppgifter.) MPN-kontot ska ha behörighet som global administratör eller kontoadministratör. 

1. Från ikonen **Inställningar väljer** du **Kontoinställningar och** sedan **Organisationsprofil.**

2. Välj **Juridiskt** och sedan På fliken **Partner** väljer du **Företagsplatser och sedan** Lägg till en **plats.**

3. Ange nödvändig information, inklusive företagsnamn, adress och kontakt för den plats som du vill lägga till i företaget.
 
1. Välj **Lägg till plats.** Detta skapar ett nytt MPN-ID för den nya platsen som du kan använda för CSP-transaktioner och incitament.

:::image type="content" source="images/legal-biz.png" alt-text="Lägg till ett nytt juridiskt företag.":::

> [!NOTE]
> När en plats har lagts till i Partnercenter kan du inte ta bort den. MPN **visas på** den vänstra menyn i Partnercenter om du har använt rätt MPN-ID för att logga in.

## <a name="add-the-registration-number-id"></a>Lägg till registreringsnummer-ID:t

Om du är en indirekt leverantör, partner för direktfakturering eller indirekt återförsäljare och du gör affärer med nya eller befintliga kunder i följande länder måste du ange registrerings-ID-nummer för din verksamhet. Om landet du gör affärer i inte visas nedan är registrerings-ID valfritt.

- Armenien 
- Azerbajdzjan 
- Vitryssland 
- Brasilien 
- Ungern 
- Indien 
- Irak 
- Kazakstan 
- Kirgizistan 
- Moldavien 
- Myanmar 
- Polen 
- Ryssland 
- Saudiarabien 
- Sydafrika 
- Sydsudan  
- Tadzjikistan 
- Thailand
- Turkiet 
- Ukraina 
- Förenade Arabemiraten 
- Uzbekistan 
- Venezuela
- Vietnam 


Mer information finns i Informationen [om registrerings-ID-nummer](reg-number-id.md)

## <a name="delete-a-location"></a>Ta bort en plats

Om du vill ta bort en plats från ditt konto måste du kontakta [partnersupporten.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b) Det är viktigt att du förstår vad som händer om du utför den här åtgärden. Borttagna platser kan inte hämtas och allt som är kopplat till det specifika MPN-ID:t känns inte längre igen eller är aktivt för ditt företag.

## <a name="change-country-of-partner-global-account"></a>Ändra land för partnerns globala konto 

1. Logga in med MPN-kontot i Partnercenter. (Dina MPN-autentiseringsuppgifter kan vara annorlunda än dina CSP-autentiseringsuppgifter.) MPN-kontot ska ha behörighet som global administratör eller kontoadministratör. 

2. På fliken **Partner** går du till **Företagsplatser** och kontrollerar listan över platser för att se till att den plats som du vill ha som din juridiska enhet visas. 
 
1. Om du vill lägga till en plats klickar du på Lägg till en plats och anger nödvändig information, inklusive företagsnamn, adress och primär kontakt för den plats som du vill lägga till i företaget. 
 
1. Välj **Ändra ditt** land bredvid **listrutan Land/region** och följ stegen. 

:::image type="content" source="images/lbp.png" alt-text="Data om juridiska affärsprofiler är tillgängliga.":::

5. Välj **Spara**.

6. MPN:s globala kontoland ändras till det nya juridiska landet.
  
## <a name="next-steps"></a>Nästa steg

- Läs mer om [verifieringsprocessen](verification-responses.md).
