---
title: Anpassa en enhets in-of-box-upplevelse
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Innan du levererar en kunds nya enhet kan du använda Windows Autopilot-profiler för att anpassa eller förkonfigurera enhetens OOBE (Out-of-Box Experience).
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 95a201c53fc2eaf230d08bb4cfdd03a5747b5c05
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246433"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Använd Windows Autopilot-profiler på nya enheter för att anpassa kundens välkomstupplevlese (OOBE, Out-Of-Box Experience)

**Lämpliga roller:** Administratörsagent | Global | Försäljningsagentens | Administratör för användarhantering

Om du hanterar kundenheter kan du behöva anpassa OOBE (Out-of-Box Experience) för kundens användare. Du kan förkonfigurera nya enheter Windows Autopilot-profiler innan du levererar enheterna till kunder och tillämpar nya profiler på enheter som kunder redan har köpt. 

Observera att OEM-tillverkare har börjat inkludera en adressetikett utanför Autopilot-enheten som visar enhetens **produktnyckel-ID (PKID).**  Den här 1-dimensionella, läsbara streckkoden ger underordnade partner ett sätt att registrera enheter för Autopilot utan att behöva packa upp enheterna och samla enhets-ID:t på ett alternativt sätt.

Den här artikeln förklarar hur du skapar och tillämpar Autopilot-profiler på enheter i Partnercenter.

Om du inte redan är bekant med Autopilot kan du läsa informationen i följande artiklar:

- [Översikt över Windows Autopilot](/windows/deployment/windows-10-auto-pilot)
- [Referensguide för Autopilot-distribution](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Översikt

Med hjälp Windows Autopilot-funktionen i Partnercenter kan du skapa anpassade profiler som ska tillämpas på kundenheter. Följande profilinställningar var tillgängliga när den här artikeln publicerades:

- Hoppa över sekretessinställningar. Den här valfria Autopilot-profilinställningen gör det möjligt för organisationer att inte fråga om sekretessinställningar under OOBE-processen.

- Inaktivera skapande av lokalt administratörskonto på enheten. Organisationer kan bestämma om användaren som ställer in enheten ska ha administratörsåtkomst när processen är klar.

- Konfigurera enheten automatiskt för arbete eller skola. Alla enheter som är registrerade med Autopilot betraktas automatiskt som arbets- eller skolenheter, så den här frågan ställs inte under OOBE-processen.

- Hoppa Cortana, OneDrive och installationssidor för OEM-registrering. Alla enheter som är registrerade med Autopilot hoppar automatiskt över dessa sidor under OOBE-processen (Out-of-Box Experience).

- Hoppa över licensavtalet (EULA). Från och Windows 10 version 1709 kan organisationer välja att hoppa över den EULA-sida som presenterades under OOBE-processen. Se [Windows autopilot-licensavtalet nedan](#windows-autopilot-eula-dismissal) för viktig information om hur du hoppar över eula-sidan under Windows installation.

Följande behörigheter och begränsningar för hantering av profiler och enheter gäller:

- CSP-partner kan fortsätta att hantera Autopilot-profiler för befintliga kunder som de har återförsäljarrelationer med, även om kunderna har tagit bort partnerns delegerade administrationsprivilegier.

- Du kan hantera befintliga enheter för kunder som du har lagt till.

- Du kan inte hantera enheter som kunden har laddat upp till Microsoft Store för företag eller Microsoft Intune-portalen.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Skapa och hantera Autopilot-profiler i Partnercenter

I Partnercenter kan du skapa Windows Autopilot-distributionsprofiler och tillämpa dem på enheter.

>[!NOTE]
>Endast administratörsagenter kan skapa och tillämpa profiler.

### <a name="create-a-new-autopilot-profile"></a>Skapa en ny Autopilot-profil

1. Välj **Kunder** på Menyn i Partnercenter och välj sedan den kund som du skapar Autopilot-profilen för.

2. På kundens informationssida väljer du **Enheter**.

3. Under **Windows Autopilot-profiler väljer** du Lägg till ny **profil.**

4. Ange profilens namn och beskrivning och konfigurera sedan OOBE-inställningarna. Välj mellan:  

   - Hoppa över sekretessinställningar i konfigurationen

   - Inaktivera lokalt administratörskonto under installationen
  
   - Hoppa automatiskt över sidor i konfigurationen<br>
        (Inkluderar *Välj automatiskt installation för arbete eller skola och* sidor för *Cortana, OneDrive och OEM-registrering)*
  
   - Hoppa över licensavtalet (EULA)<br> 
       >[!IMPORTANT] 
       >Se [Windows autopilot-licensavtalet nedan](#windows-autopilot-eula-dismissal) för viktig information om hur du hoppar över eula-sidan under Windows installation.

5. Välj **Skicka** när du är klar.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Tillämpa en Autopilot-profil på kundenheter

>[!NOTE]
>Anvisningarna nedan förutsätter att du redan har lagt till kundens enheter i Partnercenter och att du kan komma åt deras enhetslista. Om du inte redan har lagt till kundens enheter följer du anvisningarna i [Lägg](#add-devices-to-a-customers-account) till enheter till en kunds konto och följer sedan stegen nedan.

När du har skapat en Autopilot-profil för en kund kan du tillämpa den på kundens enheter.

1. Välj **Kunder** på Menyn i Partnercenter och välj sedan den kund som du skapade Autopilot-profilen för.

2. På kundens informationssida väljer du **Enheter**.

3. Under **Tillämpa profiler på enheter väljer** du de enheter eller enhetsgrupper som du vill lägga till profiler i och väljer sedan Tillämpa **profil.** Profilen som du nyss tillämpade visas i **kolumnen** Profil.

4. Följ stegen nedan för att kontrollera att profilen kommer att tillämpas på enheten.

    a.  Anslut en enhet till nätverket och aktivera den.

    b.  Kontrollera att lämpliga OOBE-skärmar (om några) visas.

    c.  När OOBE-processen stoppas återställer du enheten till fabriksinställningarna för att förbereda den för en ny användare.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Ta bort en Autopilot-profil från en kunds enhet

1. Välj **Kunder** på Menyn i Partnercenter och välj sedan den kund som du skapade Autopilot-profilen för.

2. På kundens informationssida väljer du **Enheter**.

3. Under **Tillämpa profiler på enheter väljer** du de enheter som du vill ta bort profilen från och väljer sedan Ta bort **profil.**

   >[!NOTE]
   >Om du tar bort en profil från en enhet tas inte profilen bort från listan. Om du vill ta bort en profil följer du anvisningarna i [Uppdatera eller ta bort en Autopilot-profil.](#update-or-delete-an-autopilot-profile)

### <a name="update-or-delete-an-autopilot-profile"></a>Uppdatera eller ta bort en Autopilot-profil

Om en kund vill ändra den in-of-box-upplevelsen när du har skickat enheterna till dem kan du ändra profilen i Partnercenter.

När kundens enhet ansluter till Internet laddas den senaste profilversionen ned under OOBE-processen. Varje gång en kund återställer en enhet till fabriksinställningarna hämtar enheten även den senaste profilversionen under OOBE-processen.

1. Välj **Kunder** på Menyn i Partnercenter och välj sedan den kund som vill att du ändrar en Autopilot-profil.

2. På kundens informationssida väljer du **Enheter**.

3. Under **Windows Autopilot-profiler** väljer du den profil som du behöver uppdatera. Gör de nödvändiga ändringarna och välj sedan **Skicka**.

Om du vill ta bort den här **profilen väljer du** Ta bort profil i det övre högra hörnet på sidan.

### <a name="add-devices-to-a-customers-account"></a>Lägga till enheter till en kunds konto

>[!NOTE]
>Försäljningsagenter och administratörsagenter kan lägga till enheter till en kunds konto.

Innan du kan tillämpa anpassade Autopilot-profiler på kundenheter måste du kunna komma åt kundens enhetslista.

Om du planerar att använda OEM-namn, serienummer och modellkombination bör du vara medveten om dessa begränsningar:

- Den här tuppeln fungerar bara för nyare enheter (till exempel 4 000 hash-värden) och stöds inte för hash-värden på 128b (RS2 och tidigare enheter).

- Tuppelregistreringen är fallkänslig, så data i filen måste  matcha modell- och tillverkarnamnen exakt som tillhandahålls av OEM-leverantören (maskinvaruprovidern).

Följ anvisningarna nedan för att lägga till enheter till en kunds konto i Partnercenter.

1. Välj **Kunder** på Menyn i Partnercenter och välj sedan den kund vars enheter du vill hantera.

2. På kundens informationssida väljer du **Enheter**.

3. Under **Tillämpa profiler på enheter väljer** du Lägg till **enheter.**

4. Ange ett namn på enhetslistan och välj sedan **Bläddra** för att ladda upp kundens lista (i .csv filformat) till Partnercenter.

    >[!NOTE]
    >Du bör ha fått den här .csv-filen med ditt enhetsköp. Om du inte har fått någon .csv kan du skapa en själv genom att följa stegen i Lägga till enheter [i Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Upload .csv och välj sedan **Spara**.

Om du får ett felmeddelande när du försöker ladda upp CSV-filen kontrollerar du filformatet. Du kan använda bara maskinvaruhashen, eller OEM-namnet, serienumret och modellen (i den kolumnordningen) eller produkt-ID:t för Windows. Du kan också använda exempelfilen .csv från länken bredvid Lägg till enheter **för att** skapa en enhetslista.

Din .csv bör se ut ungefär så här:

> **Enhetens serienummer, Windows produkt-ID, maskinvaruhash, tillverkarnamn, enhetsmodell**

> **{serialNumber},,,Microsoft Corporation,Surface Laptop**

>[!NOTE]
> "Tillverkarnamn" och "Enhetsmodell" är fallkänsliga.

Om du inte vet vilket värde som ska anges för Tillverkare och Enhetsmodell kan du köra det här på enheten för att samla in rätt värden:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA-avstängning

### <a name="important-information"></a>VIKTIG INFORMATION

Windows Med Autopilot kan du konfigurera anpassade installationer av Windows på enheter som du hanterar för dina kunder. Om kunden har behörighet att göra det kan du ignorera eller dölja vissa inställningsskärmar som normalt visas för användarna när de ställer in Windows, inklusive godkännandeskärmen för licensavtalet (licensavtal).

Genom att använda den här funktionen samtycker du till att förhindra eller dölja skärmar som har utformats för att ge användarna meddelanden eller godkännande av villkoren innebär att du har fått tillräckligt med medgivande och auktorisering från kunden för att dölja villkoren och att du, för din kunds räkning (oavsett om det är en organisation eller en enskild användare).  godkänn eventuella meddelanden och godkänn eventuella villkor som gäller för din kund. Detta omfattar avtal om villkoren för licensen eller meddelandet som visas för användaren om du inte utelämnar eller döljer den med hjälp av det här verktyget. Kunden får inte använda Windows på dessa enheter om kunden inte har köpt en giltig licens för programvaran från Microsoft eller dess licensierade distributörer.