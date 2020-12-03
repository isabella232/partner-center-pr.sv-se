---
title: Anpassa en enhets välkomst upplevelse
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Innan du levererar en kunds nya enhet kan du använda Windows autopilot-profiler för att anpassa eller förkonfigurera enhetens out-of-Box Experience (OOBE).
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 12057d50e4456dd2450ff497e00c89a9afa5dc4d
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96535005"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Använd Windows Autopilot-profiler på nya enheter för att anpassa kundens välkomstupplevlese (OOBE, Out-Of-Box Experience)

**Lämpliga roller**

- Administratörs agent
- Global administratör
- Försäljnings agent
- Administratör för användar hantering

Om du hanterar kund enheter kan du behöva anpassa OOBE (out-of-Box Experience) för kundens användare. Du kan förkonfigurera nya enheter med Windows autopilot-profiler innan du levererar enheterna till kunder och tillämpa nya profiler på enheter som kunder redan har köpt. 

Observera att OEM-tillverkare har börjat inklusive en leverans etikett utanför den autopilot-rutan som visar enhetens **produkt nyckel-ID (PKID)**.  Den här 1-dimensionella och läsbara streckkoden ger underordnade partner ett sätt att registrera enheter för autopilot utan att behöva avpaketera enheterna och skörda enhets-ID: t på alternativa sätt.

Den här artikeln förklarar hur du skapar och använder autopilot-profiler för enheter i Partner Center.

Om du inte redan är bekant med autopilot kan du läsa informationen i följande artiklar:

- [Översikt över Windows Autopilot](/windows/deployment/windows-10-auto-pilot)
- [Referens guide för autopilot-distribution](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Översikt

Med Windows autopilot-funktionen i Partner Center kan du skapa anpassade profiler som gäller för kund enheter. Följande profil inställningar var tillgängliga vid den tidpunkt då artikeln publicerades:

- Hoppa över sekretess inställningar. Den här valfria inställningen för autopilot-profilen gör det möjligt för organisationer att inte fråga om sekretess inställningar under OOBE-processen.

- Inaktivera skapande av lokalt administratörs konto på enheten. Organisationer kan bestämma om användaren konfigurerar enheten ska ha administratörs behörighet när processen är klar.

- Konfigurera automatiskt enheter för arbete eller skola. Alla enheter som är registrerade med autopiloten betraktas automatiskt som arbets-eller skol enheter, så den här frågan kommer inte att tillfrågas under OOBE-processen.

- Installations sidorna för att hoppa över Cortana, OneDrive och OEM-registrering. Alla enheter som är registrerade med autopiloten hoppar över dessa sidor automatiskt under processen OOBE (out-of-Box Experience).

- Hoppa över licens avtal för slutanvändare (EULA). Från och med Windows 10 version 1709 kan organisationer välja att hoppa över EULA-sidan som visas under OOBE-processen. Mer information om hur du hoppar över EULA-sidan under installationen av Windows finns i [Windows autopilot-licensavtalet](#windows-autopilot-eula-dismissal) .

Följande behörigheter och begränsningar för hantering av profiler och enheter gäller:

- CSP-partner kan fortsätta att hantera Autopilot-profiler för befintliga kunder som de har återförsäljarrelationer med, även om kunderna har tagit bort partnerns delegerade administrationsprivilegier.

- Du kan hantera befintliga enheter för kunder som du har lagt till.

- Du kan inte hantera enheter som kunden har laddat upp till Microsoft Store för företag eller Microsoft Intune-portalen.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Skapa och hantera autopilot-profiler i Partner Center

I Partner Center kan du skapa distributions profiler för Windows autopilot och tillämpa dem på enheter.

>[!NOTE]
>Endast administratörs agenter kan skapa och tillämpa profiler.

### <a name="create-a-new-autopilot-profile"></a>Skapa en ny autopilot-profil

1. Välj **kunder** från menyn Partner Center och välj sedan den kund som du vill skapa autopilot-profilen för.

2. På kundens informations sida väljer du **enheter**.

3. Under **Windows autopilot-profiler** väljer du **Lägg till ny profil**.

4. Ange profilens namn och beskrivning och konfigurera sedan OOBE-inställningarna. Välj mellan:  

   - Hoppa över sekretess inställningar i installationen

   - Inaktivera lokalt administratörs konto i installationen
  
   - Hoppa över sidor i installationen automatiskt<br>
        (Inkluderar *automatiskt Välj inställningar för arbete eller skola* och *hoppa över inställningar för Cortana, OneDrive och OEM-registrering*)
  
   - Hoppa över licens avtal för slutanvändare (EULA)<br> 
       >[!IMPORTANT] 
       >Mer information om hur du hoppar över EULA-sidan under installationen av Windows finns i [Windows autopilot-licensavtalet](#windows-autopilot-eula-dismissal) .

5. Välj **Skicka** när du är färdig.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Tillämpa en autopilot-profil på kund enheter

>[!NOTE]
>Anvisningarna nedan förutsätter att du redan har lagt till kundens enheter i Partner Center och att du har åtkomst till enhets listan. Om du inte redan har lagt till kundens enheter följer du anvisningarna i [Lägg till enheter till ett kund konto](#add-devices-to-a-customers-account) och följer sedan stegen nedan.

När du har skapat en autopilot-profil för en kund kan du använda den på kundens enheter.

1. Välj **kunder** från menyn Partner Center och välj sedan den kund som du skapade autopilot-profilen för.

2. På kundens informations sida väljer du **enheter**.

3. Under **Använd profiler på enheter** väljer du de enheter eller enhets grupper som du vill lägga till profiler i och väljer sedan **Använd profil**. Den profil du nyss använde visas i kolumnen **profil** .

4. Följ stegen nedan för att kontrol lera att profilen kommer att tillämpas på enheten.

    a.  Anslut en enhet till nätverket och aktivera den.

    b.  Kontrol lera att lämpliga OOBE-skärmar visas.

    c.  När OOBE-processen stoppas återställer du enheten till fabriks inställningarna för att förbereda den för en ny användare.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Ta bort en autopilot-profil från en kunds enhet

1. Välj **kunder** från menyn Partner Center och välj sedan den kund som du skapade autopilot-profilen för.

2. På kundens informations sida väljer du **enheter**.

3. Under **Använd profiler på enheter** väljer du de enheter som du vill ta bort profilen från och väljer sedan **ta bort profil**.

   >[!NOTE]
   >Om du tar bort en profil från en enhet tas inte profilen bort från listan. Om du vill ta bort en profil följer du anvisningarna i [Uppdatera eller ta bort en autopilot-profil](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Uppdatera eller ta bort en autopilot-profil

Om en kund vill ändra välkomst upplevelsen när du har levererat enheterna till dem kan du ändra profilen i Partner Center.

När kundens enhet ansluter till Internet hämtar den den senaste profil versionen under OOBE-processen. Varje gång en kund återställer en enhet till fabriks inställningarna kommer enheten återigen att ladda ned den senaste profil versionen under OOBE-processen.

1. Välj **kunder** från menyn Partner Center och välj sedan den kund som vill ändra en autopilot-profil.

2. På kundens informations sida väljer du **enheter**.

3. Under **Windows autopilot-profiler** väljer du den profil som du vill uppdatera. Gör de ändringar som krävs och välj sedan **Skicka**.

Om du vill ta bort profilen väljer du **ta bort profil** i det övre högra hörnet på sidan.

### <a name="add-devices-to-a-customers-account"></a>Lägga till enheter till en kunds konto

>[!NOTE]
>Försäljnings agenter och administratörs agenter kan lägga till enheter till ett kund konto.

Innan du kan använda anpassade autopilot-profiler på kund enheter måste du kunna komma åt kundens enhets lista.

Om du planerar att använda kombinationen av OEM-namn, serie nummer och modell bör du vara medveten om dessa begränsningar:

- Denna tupel fungerar bara för nyare enheter (t. ex. 4K-hashs) och stöds inte för 128B-hashar (RS2 och tidigare enheter).

- Tuple-registreringen är Skift läges känslig, så data i filen måste matcha modell-och tillverkarens namn **_exakt_* _ som anges av OEM-leverantören (maskin varu leverantören).

Följ anvisningarna nedan om du vill lägga till enheter till ett kund konto i Partner Center.

1. Välj _ *kunder** på menyn Partner Center och välj sedan den kund vars enheter du vill hantera.

2. På kundens informations sida väljer du **enheter**.

3. Under **Använd profiler på enheter** väljer du **Lägg till enheter**.

4. Ange ett namn på enhets listan och välj sedan **Bläddra** för att överföra kundens lista (i CSV-filformat) till Partner Center.

    >[!NOTE]
    >Du bör ha tagit emot den här CSV-filen med enhets köpet. Om du inte har fått en. csv-fil kan du skapa en själv genom att följa stegen i [lägga till enheter i autopilot i Windows](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Ladda upp CSV-filen och välj sedan **Spara**.

Om du får ett felmeddelande när du försöker ladda upp CSV-filen kontrollerar du filformatet. Du kan använda bara maskinvaruhashen, eller OEM-namnet, serienumret och modellen (i den kolumnordningen) eller produkt-ID:t för Windows. Du kan också använda den exempel-. csv-fil som tillhandahålls från länken bredvid **Lägg till enheter** för att skapa en enhets lista.

CSV-filen bör se ut ungefär så här:

> **Enhetens serie nummer, Windows-produkt-ID, maskinvaru-hash, tillverkarens namn, enhets modell**

> **{serialNumber},,, Microsoft Corporation, Surface laptop**

>[!NOTE]
> "Tillverkarnamn" och "enhets modell" är Skift läges känsliga.

Om du inte vet vilket värde som ska användas för tillverkarnamn och enhets modell kan du köra det på enheten för att samla in rätt värden:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Microsoft autopilot-EULA, avstängt

### <a name="important-information"></a>VIKTIG INFORMATION

Med Windows autopilot kan du konfigurera anpassade installationer av Windows på enheter som du hanterar för dina kunder. Om kunden har behörighet att göra det kan du utelämna eller dölja vissa konfigurations skärmar som normalt visas för användarna när de konfigurerar Windows, inklusive godkännande skärmen för licens avtalet (slutanvändare).

Med hjälp av den här funktionen du samtycker till att ignorera eller dölja alla skärmar som är utformade för att ge användarna ett meddelande eller godkännande av villkor innebär att du har fått tillräckligt med medgivande och tillstånd från kunden för att dölja villkor och att du, för din kunds räkning (oavsett om en organisation eller en enskild användare som fallet kan vara), samtycker till eventuella meddelanden och accepterar eventuella villkor som gäller för din kund. Detta omfattar avtals villkoren för licensen eller det meddelande som skulle visas för användaren om du inte har utelämnat eller dolt det med det här verktyget. Kunden får inte använda Windows-programvaran på dessa enheter om kunden inte har fått en giltig licens för program varan från Microsoft eller dess licensierade distributörer.