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
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="ce2d1-103">Använd Windows Autopilot-profiler på nya enheter för att anpassa kundens välkomstupplevlese (OOBE, Out-Of-Box Experience)</span><span class="sxs-lookup"><span data-stu-id="ce2d1-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="ce2d1-104">**Lämpliga roller:** Administratörsagent | Globala | Försäljningsagent | Administratör för användarhantering</span><span class="sxs-lookup"><span data-stu-id="ce2d1-104">**Appropriate roles**: Admin agent | Global admin | Sales agent | User management admin</span></span>

<span data-ttu-id="ce2d1-105">Om du hanterar kundenheter kan du behöva anpassa OOBE (Out-of-Box Experience) för kundens användare.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-105">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="ce2d1-106">Du kan förkonfigurera nya enheter med Windows Autopilot innan du levererar enheterna till kunder och tillämpar nya profiler på enheter som kunder redan har köpt.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-106">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="ce2d1-107">Observera att OEM-tillverkare har börjat inkludera en adressetikett utanför Autopilot-enheten som visar enhetens **produktnyckel-ID (PKID).**</span><span class="sxs-lookup"><span data-stu-id="ce2d1-107">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="ce2d1-108">Den här 1-dimensionella, läsbara streckkoden ger underordnade partner ett sätt att registrera enheter för Autopilot utan att behöva packa upp enheterna och samla enhets-ID:t på ett alternativt sätt.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-108">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="ce2d1-109">Den här artikeln beskriver hur du skapar och tillämpar Autopilot-profiler på enheter i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="ce2d1-110">Om du inte redan är bekant med Autopilot kan du läsa informationen i följande artiklar:</span><span class="sxs-lookup"><span data-stu-id="ce2d1-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="ce2d1-111">Översikt över Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="ce2d1-111">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="ce2d1-112">Referensguide för Autopilot-distribution</span><span class="sxs-lookup"><span data-stu-id="ce2d1-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="ce2d1-113">Översikt</span><span class="sxs-lookup"><span data-stu-id="ce2d1-113">Overview</span></span>

<span data-ttu-id="ce2d1-114">Med funktionen Windows Autopilot i Partnercenter kan du skapa anpassade profiler som gäller för kundenheter.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="ce2d1-115">Följande profilinställningar var tillgängliga när den här artikeln publicerades:</span><span class="sxs-lookup"><span data-stu-id="ce2d1-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="ce2d1-116">Hoppa över sekretessinställningar.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-116">Skip privacy settings.</span></span> <span data-ttu-id="ce2d1-117">Den här valfria Autopilot-profilinställningen gör det möjligt för organisationer att inte fråga om sekretessinställningar under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="ce2d1-118">Inaktivera skapande av lokalt administratörskonto på enheten.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="ce2d1-119">Organisationer kan bestämma om användaren som ställer in enheten ska ha administratörsåtkomst när processen är klar.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="ce2d1-120">Konfigurera automatiskt enheten för arbete eller skola.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="ce2d1-121">Alla enheter som registreras med Autopilot betraktas automatiskt som arbets- eller skolenheter, så den här frågan ställs inte under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="ce2d1-122">Hoppa över registreringsinstallationssidorna för Cortana, OneDrive och OEM.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="ce2d1-123">Alla enheter som registrerats med Autopilot hoppar automatiskt över dessa sidor under OOBE-processen (Out-of-Box Experience).</span><span class="sxs-lookup"><span data-stu-id="ce2d1-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="ce2d1-124">Hoppa över licensavtalet (EULA).</span><span class="sxs-lookup"><span data-stu-id="ce2d1-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="ce2d1-125">Från och Windows 10 version 1709 kan organisationer välja att hoppa över den EULA-sida som presenteras under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="ce2d1-126">Se [Windows Autopilot EULA nedan för](#windows-autopilot-eula-dismissal) viktig information om hur du hoppar över eula-sidan under Windows-installationen.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="ce2d1-127">Följande behörigheter och begränsningar för hantering av profiler och enheter gäller:</span><span class="sxs-lookup"><span data-stu-id="ce2d1-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="ce2d1-128">CSP-partner kan fortsätta att hantera Autopilot-profiler för befintliga kunder som de har återförsäljarrelationer med, även om kunderna har tagit bort partnerns delegerade administrationsprivilegier.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="ce2d1-129">Du kan hantera befintliga enheter för kunder som du har lagt till.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="ce2d1-130">Du kan inte hantera enheter som kunden har laddat upp till Microsoft Store för företag eller Microsoft Intune-portalen.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-130">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="ce2d1-131">Skapa och hantera Autopilot-profiler i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="ce2d1-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="ce2d1-132">I Partnercenter kan du skapa Windows Autopilot och tillämpa dem på enheter.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="ce2d1-133">Endast administratörsagenter kan skapa och tillämpa profiler.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="ce2d1-134">Skapa en ny Autopilot-profil</span><span class="sxs-lookup"><span data-stu-id="ce2d1-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="ce2d1-135">Välj **Kunder** på Menyn i Partnercenter och välj sedan den kund som du skapar Autopilot-profilen för.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="ce2d1-136">På kundens informationssida väljer du **Enheter**.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="ce2d1-137">Under **Windows Autopilot väljer du** Lägg till ny **profil.**</span><span class="sxs-lookup"><span data-stu-id="ce2d1-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="ce2d1-138">Ange profilens namn och beskrivning och konfigurera sedan OOBE-inställningarna.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="ce2d1-139">Välj mellan:</span><span class="sxs-lookup"><span data-stu-id="ce2d1-139">Choose from:</span></span>  

   - <span data-ttu-id="ce2d1-140">Hoppa över sekretessinställningar i konfigurationen</span><span class="sxs-lookup"><span data-stu-id="ce2d1-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="ce2d1-141">Inaktivera lokalt administratörskonto under installationen</span><span class="sxs-lookup"><span data-stu-id="ce2d1-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="ce2d1-142">Hoppa automatiskt över sidor i konfigurationen</span><span class="sxs-lookup"><span data-stu-id="ce2d1-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="ce2d1-143">(Inkluderar Välj *automatiskt installation för arbete eller skola och* hoppa över *installationssidorna för Cortana, OneDrive och OEM-registrering*)</span><span class="sxs-lookup"><span data-stu-id="ce2d1-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="ce2d1-144">Hoppa över licensavtalet (EULA)</span><span class="sxs-lookup"><span data-stu-id="ce2d1-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="ce2d1-145">Se [Windows Autopilot eula som avvisas](#windows-autopilot-eula-dismissal) nedan för viktig information att överväga om att hoppa över eula-sidan under Windows-installationen.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="ce2d1-146">Välj **Skicka** när du är klar.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="ce2d1-147">Tillämpa en Autopilot-profil på kundenheter</span><span class="sxs-lookup"><span data-stu-id="ce2d1-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="ce2d1-148">Anvisningarna nedan förutsätter att du redan har lagt till kundens enheter i Partnercenter och att du kan komma åt deras enhetslista.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="ce2d1-149">Om du inte redan har lagt till kundens enheter följer du anvisningarna i [Lägg](#add-devices-to-a-customers-account) till enheter till ett kundkonto och följer sedan stegen nedan.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="ce2d1-150">När du har skapat en Autopilot-profil för en kund kan du tillämpa den på kundens enheter.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="ce2d1-151">Välj **Kunder** på Partnercenter-menyn och välj sedan den kund som du skapade Autopilot-profilen för.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="ce2d1-152">På kundens informationssida väljer du **Enheter**.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="ce2d1-153">Under **Tillämpa profiler på enheter väljer** du de enheter eller enhetsgrupper som du vill lägga till profiler till och väljer sedan Tillämpa **profil.**</span><span class="sxs-lookup"><span data-stu-id="ce2d1-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="ce2d1-154">Profilen som du precis har tillämpat visas i **kolumnen** Profil.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="ce2d1-155">Följ stegen nedan för att kontrollera att profilen kommer att tillämpas på enheten.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="ce2d1-156">a.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-156">a.</span></span>  <span data-ttu-id="ce2d1-157">Anslut en enhet till nätverket och aktivera den.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="ce2d1-158">b.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-158">b.</span></span>  <span data-ttu-id="ce2d1-159">Kontrollera att lämpliga OOBE-skärmar (om några) visas.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="ce2d1-160">c.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-160">c.</span></span>  <span data-ttu-id="ce2d1-161">När OOBE-processen stoppas återställer du enheten till fabriksinställningarna för att förbereda den för en ny användare.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="ce2d1-162">Ta bort en Autopilot-profil från en kunds enhet</span><span class="sxs-lookup"><span data-stu-id="ce2d1-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="ce2d1-163">Välj **Kunder** på Partnercenter-menyn och välj sedan den kund som du skapade Autopilot-profilen för.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="ce2d1-164">På kundens informationssida väljer du **Enheter**.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="ce2d1-165">Under **Tillämpa profiler på enheter väljer** du de enheter som du vill ta bort profilen från och väljer sedan Ta bort **profil.**</span><span class="sxs-lookup"><span data-stu-id="ce2d1-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="ce2d1-166">Om du tar bort en profil från en enhet tas profilen inte bort från listan.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="ce2d1-167">Om du vill ta bort en profil följer du anvisningarna i [Uppdatera eller ta bort en Autopilot-profil.](#update-or-delete-an-autopilot-profile)</span><span class="sxs-lookup"><span data-stu-id="ce2d1-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="ce2d1-168">Uppdatera eller ta bort en Autopilot-profil</span><span class="sxs-lookup"><span data-stu-id="ce2d1-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="ce2d1-169">Om en kund vill ändra den inrutade upplevelsen när du har skickat enheterna till dem kan du ändra profilen i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="ce2d1-170">När kundens enhet ansluter till Internet laddas den senaste profilversionen ned under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="ce2d1-171">Varje gång en kund återställer en enhet till fabriksinställningarna hämtar enheten även den senaste profilversionen under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="ce2d1-172">Välj **Kunder** på Menyn i Partnercenter och välj sedan den kund som vill att du ändrar en Autopilot-profil.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="ce2d1-173">På kundens informationssida väljer du **Enheter**.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="ce2d1-174">Under **Windows Autopilot profiler** väljer du den profil som du behöver uppdatera.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="ce2d1-175">Gör de nödvändiga ändringarna och välj sedan **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="ce2d1-176">Om du vill ta bort den här **profilen väljer du** Ta bort profil i det övre högra hörnet på sidan.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="ce2d1-177">Lägga till enheter till en kunds konto</span><span class="sxs-lookup"><span data-stu-id="ce2d1-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="ce2d1-178">Försäljningsagenter och administratörsagenter kan lägga till enheter till en kunds konto.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="ce2d1-179">Innan du kan tillämpa anpassade Autopilot-profiler på kundenheter måste du kunna komma åt kundens enhetslista.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="ce2d1-180">Om du planerar att använda OEM-namn, serienummer och modellkombination bör du vara medveten om dessa begränsningar:</span><span class="sxs-lookup"><span data-stu-id="ce2d1-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="ce2d1-181">Den här tuppeln fungerar bara för nyare enheter (till exempel 4 000 hash-värden) och stöds inte för hash-värden på 128b (RS2 och tidigare enheter).</span><span class="sxs-lookup"><span data-stu-id="ce2d1-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="ce2d1-182">Tuppelregistreringen är fallkänslig, så data i filen måste  matcha modell- och tillverkarnamnen exakt som tillhandahålls av OEM-leverantören (maskinvaruprovidern).</span><span class="sxs-lookup"><span data-stu-id="ce2d1-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="ce2d1-183">Följ anvisningarna nedan för att lägga till enheter till en kunds konto i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="ce2d1-184">Välj **Kunder** på Menyn i Partnercenter och välj sedan den kund vars enheter du vill hantera.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="ce2d1-185">På kundens informationssida väljer du **Enheter**.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="ce2d1-186">Under **Tillämpa profiler på enheter väljer** du Lägg till **enheter.**</span><span class="sxs-lookup"><span data-stu-id="ce2d1-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="ce2d1-187">Ange ett namn för enhetslistan och välj sedan **Bläddra** för att ladda upp kundens lista (i CSV-filformat) till Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="ce2d1-188">Du bör ha fått den här CSV-filen med ditt enhetsköp.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="ce2d1-189">Om du inte fick någon CSV-fil kan du skapa en själv genom att följa stegen i Lägga till enheter [i Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="ce2d1-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="ce2d1-190">Ladda upp CSV-filen och välj sedan **Spara.**</span><span class="sxs-lookup"><span data-stu-id="ce2d1-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="ce2d1-191">Om du får ett felmeddelande när du försöker ladda upp CSV-filen kontrollerar du filformatet.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="ce2d1-192">Du kan använda bara maskinvaruhashen, eller OEM-namnet, serienumret och modellen (i den kolumnordningen) eller produkt-ID:t för Windows.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="ce2d1-193">Du kan också använda CSV-exempelfilen från länken bredvid Lägg till enheter för **att** skapa en enhetslista.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="ce2d1-194">CSV-filen bör se ut ungefär så här:</span><span class="sxs-lookup"><span data-stu-id="ce2d1-194">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="ce2d1-195">**Enhetens serienummer, Windows produkt-ID, maskinvaruhash, tillverkarnamn, enhetsmodell**</span><span class="sxs-lookup"><span data-stu-id="ce2d1-195">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="ce2d1-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="ce2d1-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="ce2d1-197">"Tillverkarens namn" och "Enhetsmodell" är fallkänsliga.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-197">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="ce2d1-198">Om du inte vet vilket värde som ska anges för Tillverkare och Enhetsmodell kan du köra det här på enheten för att samla in rätt värden:</span><span class="sxs-lookup"><span data-stu-id="ce2d1-198">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="ce2d1-199">Windows Autopilot EULA-uppsägning</span><span class="sxs-lookup"><span data-stu-id="ce2d1-199">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="ce2d1-200">VIKTIG INFORMATION</span><span class="sxs-lookup"><span data-stu-id="ce2d1-200">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="ce2d1-201">Windows Autopilot kan du konfigurera anpassade installationer av Windows på enheter som du hanterar för dina kunder.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-201">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="ce2d1-202">Om kunden har behörighet att göra det kan du förhindra eller dölja vissa inställningsskärmar som normalt visas för användare när de operativsystemet operativsystemet, inklusive godkännandeskärmen för EULA (licensavtal).</span><span class="sxs-lookup"><span data-stu-id="ce2d1-202">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="ce2d1-203">Genom att använda den här funktionen samtycker du till att utelämna eller dölja skärmar som är utformade för att ge användarna meddelanden eller godkännande av villkoren innebär att du har fått tillräckligt med medgivande och auktorisering från kunden för att dölja villkoren och att du, för din kunds räkning (oavsett om det är en organisation eller en enskild användare i förekommande fall), samt samtycker till eventuella meddelanden och godkänner eventuella villkor som gäller för din kund.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-203">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="ce2d1-204">Detta inkluderar avtal för licensvillkoren eller meddelandet som visas för användaren om du inte utelämnar eller döljer den med hjälp av det här verktyget.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-204">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="ce2d1-205">Kunden får inte använda Windows-programvaran på dessa enheter om kunden inte har köpt en giltig licens för programvaran från Microsoft eller dess licensierade distributörer.</span><span class="sxs-lookup"><span data-stu-id="ce2d1-205">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>