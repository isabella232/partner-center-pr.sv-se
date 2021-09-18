---
title: Slå samman ditt partnerkonto med ett annat partnerkonto
description: Lär dig hur du sammanfogar ditt partnerkonto med ett annat partnerkonto i Partnercenter – för företag som är aktiva Microsoft-partner i Partnercenter.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-account
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: 4b913754dd73f99e8aa363d257a9ac658d190b6a
ms.sourcegitcommit: 5abf065c8852a858a0aa7185176d3e117f2be7e5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/18/2021
ms.locfileid: "127958862"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a>Slå samman ditt partnerkonto med ett annat partnerkonto

**Lämpliga roller:** Kontoadministratör

Två eller flera företag som är aktiva Microsoft-partner och har konton i Partnercenter kan välja att slå samman sina konton.

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a>Vad händer när två partner väljer att slå samman sina Partnercenter-konton

- Partnerorganisationen som initierar sammanslagningen blir partnerns globala konto (PGA).

- Den inbjudna organisationens PGA blir en plats för det initierande företaget.

- Alla platser för sammanslagningskontot blir platser under PGA.

- När kontosammanslagning är klar visas både kontoinformationen, till exempel platser och användare, i PGA-profilen. Du kan inte ångra den här processen.

- Alla MPN-ID:er för platser bevaras under den här konsolideringen.

- Användarens roller tas över. Om en användare till exempel hade varit incitamentsadministratör för en viss plats skulle de fortfarande ha den rollen efter sammanslagningen och kunna se de incitament som de såg före sammanslagningen.

- Azure AD-klienter och CSP-konton slås inte samman och har ingen effekt.

- Publicerade erbjudanden och pipelinedata för säljförsäljning som är associerade med båda företagen bevaras

### <a name="view-of-merged-accounts"></a>Vy över sammanslagna konton

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Kontosammanslagning.":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a>Vad som händer om du har bjudits in för att sammanslå ditt Partnercenter-konto med ett annat Partnercenter-konto

Om du vill acceptera inbjudan att slå samman konton: · Dina MPN-ID:n och platser slås samman med PGA för partnerkontot som bjudit in dig.

- Användarna förs in i det sammanslagna kontot med sina roller intakta.

- Befintliga förmåner och kompetenser bevaras för båda företagen efter sammanslagningen fram till förnyelsen. Vid förnyelse behandlas kontona som ett företag och standardförnyelsereglerna gäller.

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a>Förstå påverkan på program och fördelar när partner väljer att slå samman konton

- Alla befintliga kompetenser (Guld/Silver), inköp (till exempel Microsoft Action Pack) och tillhörande förmåner bevaras under konsolideringen. Om båda företagen har samma kompetens men det ena är guld och det andra silveret, tilldelas kompetensen med högsta kompetensnivå och partner får en uppsättning silverfördelar och en uppsättning guldfördelar för den kompetensen fram till nästa förnyelse. 

- Högsta årsdagen för Microsoft Action Pack kommer att behållas efter sammanslagningen. Om till exempel årsdagen för företag 1 är juni 2020 för Action Pack-förnyelse och årsdagen för Action Pack-förnyelse för företag 2 är oktober 2020, kommer Microsoft att använda datumet oktober 2020 som ny årsdag för det sammanslagna företaget.

- Under kontosammanslagning och fram till nästa förnyelse behåller varje konto sina Action Pack och/eller kompetensförmåner. Vid förnyelse gäller Action Pack och regler för kompetensförnyelse.

- Vid förnyelsen implementeras förmåner som ingår i kompetensen och Action Pack för partnerföretagets globala partnerkonto:

  - Microsoft Action Pack: Partnerföretaget kommer att kunna köpa en Action Pack per partner globalt konto.

  - Kompetens: Partnerföretaget får ett paket med kärnförmåner som är kopplade till deras högsta kompetens, plus kompetensspecifika förmåner som partnern är berättigad till per partner globalt konto.

- Alla förmåner omfattas av Microsoft Partner Network [användningsguiden för förmåner.](https://partner.microsoft.com/dashboard/account/merger) Exempel: en aktiverad O365 E3-token fungerar i 12 månader efter aktiveringen. När en token har aktiverats för licenser på en klientorganisation kan dessa licenser inte flyttas till en annan klientorganisation.

- MCP-ID-associationerna för båda företagen behålls och associeras med PGA MPN-ID:t.

- Go-to-market och tekniska fördelar erbjuds som kompetenskärnförmån. Efter sammanslagningen rekommenderar vi att du kontrollerar din bank- och skatteinformation för att säkerställa korrekthet.

- Om ditt företag ingår i Azure Expert MSP behålls förmånerna fram till förnyelsen.

- Om ditt företag har fått avancerade specialiseringar behålls de på båda kontona.

- Alla software assurance-sedeln behålls på båda kontona. 

- Det finns ingen effekt på DPOR- eller PAL-associationen. Eventuella associerade intäktsbidrag börjar flöda till det nya globala partnerkontot

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a>Bjud in ett företag att slå samman sitt Partnercenter-konto med ditt Partnercenter-konto

>[!Note]
>För att kunna genomföra kontosammanslagning måste du **vara kontoadministratör** för ditt företag.

1. Välj **Inställningar på** instrumentpanelen i Partnercenter. 

2. Välj **Kontosammanslagning.**

3. Lägg till DET MPN-ID som finns **i partnerprofilen** för det konto som du vill bjuda in för att sammanslå med dig. Du måste använda partnerns globala MPN-ID. Du kan inte använda ett PLATS-MPN-ID.

4. När du väljer **Sammanfoga** skickas en inbjudan till partnerföretaget. När de accepterar din begäran kan du initiera kontosammanfogningen i Partnercenter. Om företaget avvisar din begäran om att slå samman konton kan de förklara varför de avvisade begäran. En lista över alla dina kontosammanslagningar är tillgänglig för dig under **Sammanslagningshistorik.**
 
### <a name="example-of-two-companies-merging-accounts"></a>Exempel på två företag som slår samman konton

1. Contoso, Ltd. har 

    a. ett [globalt MPN-ID för 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) och en underordnad plats [MPN-ID:n för 2222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).
  
    b. en Azure AD-klientorganisation = @contoso.com
 
    c. en guldkompetens som upphör att gälla den 1 oktober 2020
2. Fabrikam, Inc. har
 
    a. ett globalt MPN-ID 3333333 och två MPN-ID:n för underordnade platser 4444444 och 5555555

    b.  en Azure AD-klientorganisation = @fabrikam.com

    c.  två guldkompetenser som upphör den 1 december 2020
3.  Contoso köper Fabrikam och går till [Partnercenter för att](https://partner.microsoft.com/dashboard/account/merger) initiera en sammanslagningsbegäran.
4.  Fabrikam loggar in på Partnercenter och går till samma sida som Contoso gjorde i steg #3, för att godkänna Contosos begäran.
5.  Contoso granskar informationen om sammanslagningen på samma sida och ger en bekräftelse för att fortsätta med kontosammanslagningen.
6.  Efter sammanslagningen visas företagskontot som:

    a.  Ett företag med namnet Contoso med ett globalt MPN-ID på 1111111 och 4 underordnade plats-MPN-ID:n för 2222222, 3333333, 4444444 och 5555555
    
    b.  Den kommer att ha två Azure AD-klienter ( @contoso.com + ) som har åtkomst till samma @fabrikam.com Partnercenter-konto
    
    c.  Det kommer att ha två kompetensförmåner, ett som upphör den 1 oktober 2020 och ett annat som upphör att gälla den 1 december 2020. De kommer att kunna förnyas som ett paket med enskilda kompetensförmåner den 1 december 2020. När de förnyas behåller Contoso alla tre kompetenserna även om de bara kan underhålla ett enda förmånspaket.
    
7.  Contosos administratörer fortsätter att hantera Partner Center-roller @contoso.com för användare. Fabrikams administratörer fortsätter att hantera Partner Center-roller @fabrikam.com för användare. Contosos administratörer kan bara administrera Fabrikams användare om de bjuds in som gäst till Fabrikams klientorganisation.
8.  Contoso kan välja att ignorera klientorganisationen och @fabrikam.com återutgåva Fabrikam-anställdas nya @contoso.com autentiseringsuppgifter med nya roller och behörigheter.

## <a name="next-steps"></a>Nästa steg

- [Tilldela användarroller och -behörigheter](permissions-overview.md)

- [Verifiera din partnerprofilinformation](update-your-partner-profile.md)

- [Lägg Azure Partner Shared Services så att partner kan köpa Azure-prenumerationer för eget bruk](shared-services.md)
