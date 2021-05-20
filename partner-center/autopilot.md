---
title: Anpassa en enhets out-of-box-upplevelse
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Innan du levererar en kunds nya enhet kan du använda Windows Autopilot för att anpassa eller förkonfigurera enhetens färdiga upplevelse (OOBE).
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149833"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Använd Windows Autopilot-profiler på nya enheter för att anpassa kundens välkomstupplevlese (OOBE, Out-Of-Box Experience)

**Lämpliga roller:** Administratörsagent | Globala | Försäljningsagent | Administratör för användarhantering

Om du hanterar kundenheter kan du behöva anpassa OOBE (Out-of-Box Experience) för kundens användare. Du kan förkonfigurera nya enheter med Windows Autopilot innan du levererar enheterna till kunder och tillämpar nya profiler på enheter som kunder redan har köpt. 

Observera att OEM-tillverkare har börjat inkludera en adressetikett utanför Autopilot-enheten som visar enhetens **produktnyckel-ID (PKID).**  Den här 1-dimensionella, läsbara streckkoden ger underordnade partner ett sätt att registrera enheter för Autopilot utan att behöva packa upp enheterna och samla enhets-ID:t på ett alternativt sätt.

Den här artikeln beskriver hur du skapar och tillämpar Autopilot-profiler på enheter i Partnercenter.

Om du inte redan är bekant med Autopilot kan du läsa informationen i följande artiklar:

- [Översikt över Windows Autopilot](/windows/deployment/windows-10-auto-pilot)
- [Referensguide för Autopilot-distribution](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Översikt

Med funktionen Windows Autopilot i Partnercenter kan du skapa anpassade profiler som gäller för kundenheter. Följande profilinställningar var tillgängliga när den här artikeln publicerades:

- Hoppa över sekretessinställningar. Den här valfria Autopilot-profilinställningen gör det möjligt för organisationer att inte fråga om sekretessinställningar under OOBE-processen.

- Inaktivera skapande av lokalt administratörskonto på enheten. Organisationer kan bestämma om användaren som ställer in enheten ska ha administratörsåtkomst när processen är klar.

- Konfigurera automatiskt enheten för arbete eller skola. Alla enheter som registreras med Autopilot betraktas automatiskt som arbets- eller skolenheter, så den här frågan ställs inte under OOBE-processen.

- Hoppa över registreringsinstallationssidorna för Cortana, OneDrive och OEM. Alla enheter som registrerats med Autopilot hoppar automatiskt över dessa sidor under OOBE-processen (Out-of-Box Experience).

- Hoppa över licensavtalet (EULA). Från och Windows 10 version 1709 kan organisationer välja att hoppa över den EULA-sida som presenteras under OOBE-processen. Se [Windows Autopilot EULA nedan för](#windows-autopilot-eula-dismissal) viktig information om hur du hoppar över eula-sidan under Windows-installationen.

Följande behörigheter och begränsningar för hantering av profiler och enheter gäller:

- CSP-partner kan fortsätta att hantera Autopilot-profiler för befintliga kunder som de har återförsäljarrelationer med, även om kunderna har tagit bort partnerns delegerade administrationsprivilegier.

- Du kan hantera befintliga enheter för kunder som du har lagt till.

- Du kan inte hantera enheter som kunden har laddat upp till Microsoft Store för företag eller Microsoft Intune-portalen.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Skapa och hantera Autopilot-profiler i Partnercenter

I Partnercenter kan du skapa Windows Autopilot och tillämpa dem på enheter.

>[!NOTE]
>Endast administratörsagenter kan skapa och tillämpa profiler.

### <a name="create-a-new-autopilot-profile"></a>Skapa en ny Autopilot-profil

1. Välj **Kunder** på Menyn i Partnercenter och välj sedan den kund som du skapar Autopilot-profilen för.

2. På kundens informationssida väljer du **Enheter**.

3. Under **Windows Autopilot väljer du** Lägg till ny **profil.**

4. Ange profilens namn och beskrivning och konfigurera sedan OOBE-inställningarna. Välj mellan:  

   - Hoppa över sekretessinställningar i konfigurationen

   - Inaktivera lokalt administratörskonto under installationen
  
   - Hoppa automatiskt över sidor i konfigurationen<br>
        (Inkluderar Välj *automatiskt installation för arbete eller skola och* hoppa över *installationssidorna för Cortana, OneDrive och OEM-registrering*)
  
   - Hoppa över licensavtalet (EULA)<br> 
       >[!IMPORTANT] 
       >Se [Windows Autopilot eula som avvisas](#windows-autopilot-eula-dismissal) nedan för viktig information att överväga om att hoppa över eula-sidan under Windows-installationen.

5. Välj **Skicka** när du är klar.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Tillämpa en Autopilot-profil på kundenheter

>[!NOTE]
>Anvisningarna nedan förutsätter att du redan har lagt till kundens enheter i Partnercenter och att du kan komma åt deras enhetslista. Om du inte redan har lagt till kundens enheter följer du anvisningarna i [Lägg](#add-devices-to-a-customers-account) till enheter till ett kundkonto och följer sedan stegen nedan.

När du har skapat en Autopilot-profil för en kund kan du tillämpa den på kundens enheter.

1. Välj **Kunder** på Partnercenter-menyn och välj sedan den kund som du skapade Autopilot-profilen för.

2. På kundens informationssida väljer du **Enheter**.

3. Under **Tillämpa profiler på enheter väljer** du de enheter eller enhetsgrupper som du vill lägga till profiler till och väljer sedan Tillämpa **profil.** Profilen som du precis har tillämpat visas i **kolumnen** Profil.

4. Följ stegen nedan för att kontrollera att profilen kommer att tillämpas på enheten.

    a.  Anslut en enhet till nätverket och aktivera den.

    b.  Kontrollera att lämpliga OOBE-skärmar (om några) visas.

    c.  När OOBE-processen stoppas återställer du enheten till fabriksinställningarna för att förbereda den för en ny användare.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Ta bort en Autopilot-profil från en kunds enhet

1. Välj **Kunder** på Partnercenter-menyn och välj sedan den kund som du skapade Autopilot-profilen för.

2. På kundens informationssida väljer du **Enheter**.

3. Under **Tillämpa profiler på enheter väljer** du de enheter som du vill ta bort profilen från och väljer sedan Ta bort **profil.**

   >[!NOTE]
   >Om du tar bort en profil från en enhet tas profilen inte bort från listan. Om du vill ta bort en profil följer du anvisningarna i [Uppdatera eller ta bort en Autopilot-profil.](#update-or-delete-an-autopilot-profile)

### <a name="update-or-delete-an-autopilot-profile"></a>Uppdatera eller ta bort en Autopilot-profil

Om en kund vill ändra den inrutade upplevelsen när du har skickat enheterna till dem kan du ändra profilen i Partnercenter.

När kundens enhet ansluter till Internet laddas den senaste profilversionen ned under OOBE-processen. Varje gång en kund återställer en enhet till fabriksinställningarna hämtar enheten även den senaste profilversionen under OOBE-processen.

1. Välj **Kunder** på Menyn i Partnercenter och välj sedan den kund som vill att du ändrar en Autopilot-profil.

2. På kundens informationssida väljer du **Enheter**.

3. Under **Windows Autopilot profiler** väljer du den profil som du behöver uppdatera. Gör de nödvändiga ändringarna och välj sedan **Skicka**.

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

4. Ange ett namn för enhetslistan och välj sedan **Bläddra** för att ladda upp kundens lista (i CSV-filformat) till Partnercenter.

    >[!NOTE]
    >Du bör ha fått den här CSV-filen med ditt enhetsköp. Om du inte fick någon CSV-fil kan du skapa en själv genom att följa stegen i Lägga till enheter [i Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Ladda upp CSV-filen och välj sedan **Spara.**

Om du får ett felmeddelande när du försöker ladda upp CSV-filen kontrollerar du filformatet. Du kan använda bara maskinvaruhashen, eller OEM-namnet, serienumret och modellen (i den kolumnordningen) eller produkt-ID:t för Windows. Du kan också använda CSV-exempelfilen från länken bredvid Lägg till enheter för **att** skapa en enhetslista.

CSV-filen bör se ut ungefär så här:

> **Enhetens serienummer, Windows produkt-ID, maskinvaruhash, tillverkarnamn, enhetsmodell**

> **{serialNumber},,,Microsoft Corporation,Surface Laptop**

>[!NOTE]
> "Tillverkarens namn" och "Enhetsmodell" är fallkänsliga.

Om du inte vet vilket värde som ska anges för Tillverkare och Enhetsmodell kan du köra det här på enheten för att samla in rätt värden:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA-uppsägning

### <a name="important-information"></a>VIKTIG INFORMATION

Windows Autopilot kan du konfigurera anpassade installationer av Windows på enheter som du hanterar för dina kunder. Om kunden har behörighet att göra det kan du förhindra eller dölja vissa inställningsskärmar som normalt visas för användare när de operativsystemet operativsystemet, inklusive godkännandeskärmen för EULA (licensavtal).

Genom att använda den här funktionen samtycker du till att utelämna eller dölja skärmar som är utformade för att ge användarna meddelanden eller godkännande av villkoren innebär att du har fått tillräckligt med medgivande och auktorisering från kunden för att dölja villkoren och att du, för din kunds räkning (oavsett om det är en organisation eller en enskild användare i förekommande fall), samt samtycker till eventuella meddelanden och godkänner eventuella villkor som gäller för din kund. Detta inkluderar avtal för licensvillkoren eller meddelandet som visas för användaren om du inte utelämnar eller döljer den med hjälp av det här verktyget. Kunden får inte använda Windows-programvaran på dessa enheter om kunden inte har köpt en giltig licens för programvaran från Microsoft eller dess licensierade distributörer.