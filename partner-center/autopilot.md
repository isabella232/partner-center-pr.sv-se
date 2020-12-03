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
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="c9490-103">Använd Windows Autopilot-profiler på nya enheter för att anpassa kundens välkomstupplevlese (OOBE, Out-Of-Box Experience)</span><span class="sxs-lookup"><span data-stu-id="c9490-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="c9490-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="c9490-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c9490-105">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="c9490-105">Admin agent</span></span>
- <span data-ttu-id="c9490-106">Global administratör</span><span class="sxs-lookup"><span data-stu-id="c9490-106">Global admin</span></span>
- <span data-ttu-id="c9490-107">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="c9490-107">Sales agent</span></span>
- <span data-ttu-id="c9490-108">Administratör för användar hantering</span><span class="sxs-lookup"><span data-stu-id="c9490-108">User management admin</span></span>

<span data-ttu-id="c9490-109">Om du hanterar kund enheter kan du behöva anpassa OOBE (out-of-Box Experience) för kundens användare.</span><span class="sxs-lookup"><span data-stu-id="c9490-109">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="c9490-110">Du kan förkonfigurera nya enheter med Windows autopilot-profiler innan du levererar enheterna till kunder och tillämpa nya profiler på enheter som kunder redan har köpt.</span><span class="sxs-lookup"><span data-stu-id="c9490-110">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="c9490-111">Observera att OEM-tillverkare har börjat inklusive en leverans etikett utanför den autopilot-rutan som visar enhetens **produkt nyckel-ID (PKID)**.</span><span class="sxs-lookup"><span data-stu-id="c9490-111">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="c9490-112">Den här 1-dimensionella och läsbara streckkoden ger underordnade partner ett sätt att registrera enheter för autopilot utan att behöva avpaketera enheterna och skörda enhets-ID: t på alternativa sätt.</span><span class="sxs-lookup"><span data-stu-id="c9490-112">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="c9490-113">Den här artikeln förklarar hur du skapar och använder autopilot-profiler för enheter i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c9490-113">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="c9490-114">Om du inte redan är bekant med autopilot kan du läsa informationen i följande artiklar:</span><span class="sxs-lookup"><span data-stu-id="c9490-114">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="c9490-115">Översikt över Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="c9490-115">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="c9490-116">Referens guide för autopilot-distribution</span><span class="sxs-lookup"><span data-stu-id="c9490-116">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="c9490-117">Översikt</span><span class="sxs-lookup"><span data-stu-id="c9490-117">Overview</span></span>

<span data-ttu-id="c9490-118">Med Windows autopilot-funktionen i Partner Center kan du skapa anpassade profiler som gäller för kund enheter.</span><span class="sxs-lookup"><span data-stu-id="c9490-118">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="c9490-119">Följande profil inställningar var tillgängliga vid den tidpunkt då artikeln publicerades:</span><span class="sxs-lookup"><span data-stu-id="c9490-119">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="c9490-120">Hoppa över sekretess inställningar.</span><span class="sxs-lookup"><span data-stu-id="c9490-120">Skip privacy settings.</span></span> <span data-ttu-id="c9490-121">Den här valfria inställningen för autopilot-profilen gör det möjligt för organisationer att inte fråga om sekretess inställningar under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="c9490-121">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="c9490-122">Inaktivera skapande av lokalt administratörs konto på enheten.</span><span class="sxs-lookup"><span data-stu-id="c9490-122">Disable local admin account creation on the device.</span></span> <span data-ttu-id="c9490-123">Organisationer kan bestämma om användaren konfigurerar enheten ska ha administratörs behörighet när processen är klar.</span><span class="sxs-lookup"><span data-stu-id="c9490-123">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="c9490-124">Konfigurera automatiskt enheter för arbete eller skola.</span><span class="sxs-lookup"><span data-stu-id="c9490-124">Automatically set up device for work or school.</span></span> <span data-ttu-id="c9490-125">Alla enheter som är registrerade med autopiloten betraktas automatiskt som arbets-eller skol enheter, så den här frågan kommer inte att tillfrågas under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="c9490-125">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="c9490-126">Installations sidorna för att hoppa över Cortana, OneDrive och OEM-registrering.</span><span class="sxs-lookup"><span data-stu-id="c9490-126">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="c9490-127">Alla enheter som är registrerade med autopiloten hoppar över dessa sidor automatiskt under processen OOBE (out-of-Box Experience).</span><span class="sxs-lookup"><span data-stu-id="c9490-127">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="c9490-128">Hoppa över licens avtal för slutanvändare (EULA).</span><span class="sxs-lookup"><span data-stu-id="c9490-128">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="c9490-129">Från och med Windows 10 version 1709 kan organisationer välja att hoppa över EULA-sidan som visas under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="c9490-129">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="c9490-130">Mer information om hur du hoppar över EULA-sidan under installationen av Windows finns i [Windows autopilot-licensavtalet](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="c9490-130">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="c9490-131">Följande behörigheter och begränsningar för hantering av profiler och enheter gäller:</span><span class="sxs-lookup"><span data-stu-id="c9490-131">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="c9490-132">CSP-partner kan fortsätta att hantera Autopilot-profiler för befintliga kunder som de har återförsäljarrelationer med, även om kunderna har tagit bort partnerns delegerade administrationsprivilegier.</span><span class="sxs-lookup"><span data-stu-id="c9490-132">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="c9490-133">Du kan hantera befintliga enheter för kunder som du har lagt till.</span><span class="sxs-lookup"><span data-stu-id="c9490-133">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="c9490-134">Du kan inte hantera enheter som kunden har laddat upp till Microsoft Store för företag eller Microsoft Intune-portalen.</span><span class="sxs-lookup"><span data-stu-id="c9490-134">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="c9490-135">Skapa och hantera autopilot-profiler i Partner Center</span><span class="sxs-lookup"><span data-stu-id="c9490-135">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="c9490-136">I Partner Center kan du skapa distributions profiler för Windows autopilot och tillämpa dem på enheter.</span><span class="sxs-lookup"><span data-stu-id="c9490-136">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="c9490-137">Endast administratörs agenter kan skapa och tillämpa profiler.</span><span class="sxs-lookup"><span data-stu-id="c9490-137">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="c9490-138">Skapa en ny autopilot-profil</span><span class="sxs-lookup"><span data-stu-id="c9490-138">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="c9490-139">Välj **kunder** från menyn Partner Center och välj sedan den kund som du vill skapa autopilot-profilen för.</span><span class="sxs-lookup"><span data-stu-id="c9490-139">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="c9490-140">På kundens informations sida väljer du **enheter**.</span><span class="sxs-lookup"><span data-stu-id="c9490-140">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="c9490-141">Under **Windows autopilot-profiler** väljer du **Lägg till ny profil**.</span><span class="sxs-lookup"><span data-stu-id="c9490-141">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="c9490-142">Ange profilens namn och beskrivning och konfigurera sedan OOBE-inställningarna.</span><span class="sxs-lookup"><span data-stu-id="c9490-142">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="c9490-143">Välj mellan:</span><span class="sxs-lookup"><span data-stu-id="c9490-143">Choose from:</span></span>  

   - <span data-ttu-id="c9490-144">Hoppa över sekretess inställningar i installationen</span><span class="sxs-lookup"><span data-stu-id="c9490-144">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="c9490-145">Inaktivera lokalt administratörs konto i installationen</span><span class="sxs-lookup"><span data-stu-id="c9490-145">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="c9490-146">Hoppa över sidor i installationen automatiskt</span><span class="sxs-lookup"><span data-stu-id="c9490-146">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="c9490-147">(Inkluderar *automatiskt Välj inställningar för arbete eller skola* och *hoppa över inställningar för Cortana, OneDrive och OEM-registrering*)</span><span class="sxs-lookup"><span data-stu-id="c9490-147">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="c9490-148">Hoppa över licens avtal för slutanvändare (EULA)</span><span class="sxs-lookup"><span data-stu-id="c9490-148">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="c9490-149">Mer information om hur du hoppar över EULA-sidan under installationen av Windows finns i [Windows autopilot-licensavtalet](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="c9490-149">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="c9490-150">Välj **Skicka** när du är färdig.</span><span class="sxs-lookup"><span data-stu-id="c9490-150">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="c9490-151">Tillämpa en autopilot-profil på kund enheter</span><span class="sxs-lookup"><span data-stu-id="c9490-151">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="c9490-152">Anvisningarna nedan förutsätter att du redan har lagt till kundens enheter i Partner Center och att du har åtkomst till enhets listan.</span><span class="sxs-lookup"><span data-stu-id="c9490-152">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="c9490-153">Om du inte redan har lagt till kundens enheter följer du anvisningarna i [Lägg till enheter till ett kund konto](#add-devices-to-a-customers-account) och följer sedan stegen nedan.</span><span class="sxs-lookup"><span data-stu-id="c9490-153">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="c9490-154">När du har skapat en autopilot-profil för en kund kan du använda den på kundens enheter.</span><span class="sxs-lookup"><span data-stu-id="c9490-154">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="c9490-155">Välj **kunder** från menyn Partner Center och välj sedan den kund som du skapade autopilot-profilen för.</span><span class="sxs-lookup"><span data-stu-id="c9490-155">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="c9490-156">På kundens informations sida väljer du **enheter**.</span><span class="sxs-lookup"><span data-stu-id="c9490-156">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="c9490-157">Under **Använd profiler på enheter** väljer du de enheter eller enhets grupper som du vill lägga till profiler i och väljer sedan **Använd profil**.</span><span class="sxs-lookup"><span data-stu-id="c9490-157">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="c9490-158">Den profil du nyss använde visas i kolumnen **profil** .</span><span class="sxs-lookup"><span data-stu-id="c9490-158">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="c9490-159">Följ stegen nedan för att kontrol lera att profilen kommer att tillämpas på enheten.</span><span class="sxs-lookup"><span data-stu-id="c9490-159">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="c9490-160">a.</span><span class="sxs-lookup"><span data-stu-id="c9490-160">a.</span></span>  <span data-ttu-id="c9490-161">Anslut en enhet till nätverket och aktivera den.</span><span class="sxs-lookup"><span data-stu-id="c9490-161">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="c9490-162">b.</span><span class="sxs-lookup"><span data-stu-id="c9490-162">b.</span></span>  <span data-ttu-id="c9490-163">Kontrol lera att lämpliga OOBE-skärmar visas.</span><span class="sxs-lookup"><span data-stu-id="c9490-163">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="c9490-164">c.</span><span class="sxs-lookup"><span data-stu-id="c9490-164">c.</span></span>  <span data-ttu-id="c9490-165">När OOBE-processen stoppas återställer du enheten till fabriks inställningarna för att förbereda den för en ny användare.</span><span class="sxs-lookup"><span data-stu-id="c9490-165">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="c9490-166">Ta bort en autopilot-profil från en kunds enhet</span><span class="sxs-lookup"><span data-stu-id="c9490-166">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="c9490-167">Välj **kunder** från menyn Partner Center och välj sedan den kund som du skapade autopilot-profilen för.</span><span class="sxs-lookup"><span data-stu-id="c9490-167">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="c9490-168">På kundens informations sida väljer du **enheter**.</span><span class="sxs-lookup"><span data-stu-id="c9490-168">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="c9490-169">Under **Använd profiler på enheter** väljer du de enheter som du vill ta bort profilen från och väljer sedan **ta bort profil**.</span><span class="sxs-lookup"><span data-stu-id="c9490-169">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="c9490-170">Om du tar bort en profil från en enhet tas inte profilen bort från listan.</span><span class="sxs-lookup"><span data-stu-id="c9490-170">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="c9490-171">Om du vill ta bort en profil följer du anvisningarna i [Uppdatera eller ta bort en autopilot-profil](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="c9490-171">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="c9490-172">Uppdatera eller ta bort en autopilot-profil</span><span class="sxs-lookup"><span data-stu-id="c9490-172">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="c9490-173">Om en kund vill ändra välkomst upplevelsen när du har levererat enheterna till dem kan du ändra profilen i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c9490-173">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="c9490-174">När kundens enhet ansluter till Internet hämtar den den senaste profil versionen under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="c9490-174">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="c9490-175">Varje gång en kund återställer en enhet till fabriks inställningarna kommer enheten återigen att ladda ned den senaste profil versionen under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="c9490-175">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="c9490-176">Välj **kunder** från menyn Partner Center och välj sedan den kund som vill ändra en autopilot-profil.</span><span class="sxs-lookup"><span data-stu-id="c9490-176">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="c9490-177">På kundens informations sida väljer du **enheter**.</span><span class="sxs-lookup"><span data-stu-id="c9490-177">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="c9490-178">Under **Windows autopilot-profiler** väljer du den profil som du vill uppdatera.</span><span class="sxs-lookup"><span data-stu-id="c9490-178">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="c9490-179">Gör de ändringar som krävs och välj sedan **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="c9490-179">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="c9490-180">Om du vill ta bort profilen väljer du **ta bort profil** i det övre högra hörnet på sidan.</span><span class="sxs-lookup"><span data-stu-id="c9490-180">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="c9490-181">Lägga till enheter till en kunds konto</span><span class="sxs-lookup"><span data-stu-id="c9490-181">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="c9490-182">Försäljnings agenter och administratörs agenter kan lägga till enheter till ett kund konto.</span><span class="sxs-lookup"><span data-stu-id="c9490-182">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="c9490-183">Innan du kan använda anpassade autopilot-profiler på kund enheter måste du kunna komma åt kundens enhets lista.</span><span class="sxs-lookup"><span data-stu-id="c9490-183">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="c9490-184">Om du planerar att använda kombinationen av OEM-namn, serie nummer och modell bör du vara medveten om dessa begränsningar:</span><span class="sxs-lookup"><span data-stu-id="c9490-184">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="c9490-185">Denna tupel fungerar bara för nyare enheter (t. ex. 4K-hashs) och stöds inte för 128B-hashar (RS2 och tidigare enheter).</span><span class="sxs-lookup"><span data-stu-id="c9490-185">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="c9490-186">Tuple-registreringen är Skift läges känslig, så data i filen måste matcha modell-och tillverkarens namn \**_exakt_* _ som anges av OEM-leverantören (maskin varu leverantören).</span><span class="sxs-lookup"><span data-stu-id="c9490-186">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names \**_exactly_* _ as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="c9490-187">Följ anvisningarna nedan om du vill lägga till enheter till ett kund konto i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c9490-187">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="c9490-188">Välj _ *kunder*\* på menyn Partner Center och välj sedan den kund vars enheter du vill hantera.</span><span class="sxs-lookup"><span data-stu-id="c9490-188">Select _ *Customers*\* from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="c9490-189">På kundens informations sida väljer du **enheter**.</span><span class="sxs-lookup"><span data-stu-id="c9490-189">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="c9490-190">Under **Använd profiler på enheter** väljer du **Lägg till enheter**.</span><span class="sxs-lookup"><span data-stu-id="c9490-190">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="c9490-191">Ange ett namn på enhets listan och välj sedan **Bläddra** för att överföra kundens lista (i CSV-filformat) till Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c9490-191">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="c9490-192">Du bör ha tagit emot den här CSV-filen med enhets köpet.</span><span class="sxs-lookup"><span data-stu-id="c9490-192">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="c9490-193">Om du inte har fått en. csv-fil kan du skapa en själv genom att följa stegen i [lägga till enheter i autopilot i Windows](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="c9490-193">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="c9490-194">Ladda upp CSV-filen och välj sedan **Spara**.</span><span class="sxs-lookup"><span data-stu-id="c9490-194">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="c9490-195">Om du får ett felmeddelande när du försöker ladda upp CSV-filen kontrollerar du filformatet.</span><span class="sxs-lookup"><span data-stu-id="c9490-195">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="c9490-196">Du kan använda bara maskinvaruhashen, eller OEM-namnet, serienumret och modellen (i den kolumnordningen) eller produkt-ID:t för Windows.</span><span class="sxs-lookup"><span data-stu-id="c9490-196">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="c9490-197">Du kan också använda den exempel-. csv-fil som tillhandahålls från länken bredvid **Lägg till enheter** för att skapa en enhets lista.</span><span class="sxs-lookup"><span data-stu-id="c9490-197">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="c9490-198">CSV-filen bör se ut ungefär så här:</span><span class="sxs-lookup"><span data-stu-id="c9490-198">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="c9490-199">**Enhetens serie nummer, Windows-produkt-ID, maskinvaru-hash, tillverkarens namn, enhets modell**</span><span class="sxs-lookup"><span data-stu-id="c9490-199">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="c9490-200">**{serialNumber},,, Microsoft Corporation, Surface laptop**</span><span class="sxs-lookup"><span data-stu-id="c9490-200">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="c9490-201">"Tillverkarnamn" och "enhets modell" är Skift läges känsliga.</span><span class="sxs-lookup"><span data-stu-id="c9490-201">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="c9490-202">Om du inte vet vilket värde som ska användas för tillverkarnamn och enhets modell kan du köra det på enheten för att samla in rätt värden:</span><span class="sxs-lookup"><span data-stu-id="c9490-202">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="c9490-203">Microsoft autopilot-EULA, avstängt</span><span class="sxs-lookup"><span data-stu-id="c9490-203">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="c9490-204">VIKTIG INFORMATION</span><span class="sxs-lookup"><span data-stu-id="c9490-204">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="c9490-205">Med Windows autopilot kan du konfigurera anpassade installationer av Windows på enheter som du hanterar för dina kunder.</span><span class="sxs-lookup"><span data-stu-id="c9490-205">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="c9490-206">Om kunden har behörighet att göra det kan du utelämna eller dölja vissa konfigurations skärmar som normalt visas för användarna när de konfigurerar Windows, inklusive godkännande skärmen för licens avtalet (slutanvändare).</span><span class="sxs-lookup"><span data-stu-id="c9490-206">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="c9490-207">Med hjälp av den här funktionen du samtycker till att ignorera eller dölja alla skärmar som är utformade för att ge användarna ett meddelande eller godkännande av villkor innebär att du har fått tillräckligt med medgivande och tillstånd från kunden för att dölja villkor och att du, för din kunds räkning (oavsett om en organisation eller en enskild användare som fallet kan vara), samtycker till eventuella meddelanden och accepterar eventuella villkor som gäller för din kund.</span><span class="sxs-lookup"><span data-stu-id="c9490-207">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="c9490-208">Detta omfattar avtals villkoren för licensen eller det meddelande som skulle visas för användaren om du inte har utelämnat eller dolt det med det här verktyget.</span><span class="sxs-lookup"><span data-stu-id="c9490-208">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="c9490-209">Kunden får inte använda Windows-programvaran på dessa enheter om kunden inte har fått en giltig licens för program varan från Microsoft eller dess licensierade distributörer.</span><span class="sxs-lookup"><span data-stu-id="c9490-209">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>