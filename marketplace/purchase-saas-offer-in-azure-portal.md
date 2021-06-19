---
title: Så här köper du ett SaaS-erbjudande i Azure Portal
description: Lär dig hur du hittar och köper ett SaaS-erbjudande i Azure Portal.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/04/2021
ms.openlocfilehash: b73a9acb7b9cf9eee1151de1f8e45f6fd6ef256f
ms.sourcegitcommit: 8511fec63961d8c77a4d1eea3e3f1d37cdea46c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/19/2021
ms.locfileid: "112373495"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Köpa ett SaaS-erbjudande i Azure Portal

Den här artikeln beskriver de olika alternativen och kraven för att söka efter, prova och köpa ett SaaS-erbjudande (programvara som en tjänst) från Azure Portal.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS erbjuder identifiering i Azure Portal

När du är i Azure Portal finns det några sätt att begränsa sökningen för att fokusera på SaaS-erbjudanden.

### <a name="narrowing-your-search"></a>Begränsa sökningen

På startsidan under **Azure-tjänster väljer** **du + Skapa en resurs** eller **Marketplace.** Eller använd genvägen **G + N** var som helst på plattformen.

- Begränsa resultatet till SaaS-erbjudanden med filtret **Erbjudandetyp** och välj sedan **SaaS**.
- Använd global sökning i det övre navigeringsområdet för att hitta ett specifikt SaaS-erbjudande.

Hitta ett [privat SaaS-erbjudande](/marketplace/private-offers) genom att välja banderollen överst på **Marketplace-startsidan.** Alla erbjudanden eller planer är inte tillgängliga i alla geografiska områden och vissa kanske bara visas för vissa klienter.

Den filtrerade vyn visar varje tillgängligt SaaS-erbjudande som representeras av en rubrik. Välj en för att se produktinformationssidan. Detta omfattar följande avsnitt:

- Översikt – information om tjänsten, marknadsförings- och utbildningsmaterial
- Planer + priser – varje erbjudande innehåller minst en plan med olika faktureringsvillkor och priser
- Användningsinformation + support – omfattar utgivar-ID, erbjudande-ID och plan-ID
- Klassificering och recensioner av det specifika SaaS-erbjudandet

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Tillgängliga faktureringsmodeller (planer/SKU:er) för SaaS-erbjudanden

Varje SaaS-erbjudande har en eller flera planer. Varje erbjudande har en associerad prismodell: fast pris eller per användare. Varje planpris är en återkommande avgift som kan vara noll dollar (alla listade priser är endast till exempel och är inte avsedda att återspegla faktiska kostnader). Den här avgiften är antingen ett fast pris eller ett pris per användare. Typer av planer som är tillgängliga:

- **Månadsplaner –** återkommande månadsavgift; fast avgift eller månatlig avgift per användare som betalas per månad. När perioden är slut förnyas planen automatiskt.
- **Årliga planer –** återkommande årlig avgift; fast avgift eller årlig avgift per användare som betalas vid en årlig upprepning. När perioden är slut förnyas planen automatiskt.
- **Anpassade mätare** – tillsammans med de återkommande avgifterna kan en plan för fast pris även innehålla valfria anpassade mätdimensioner för överförbrukningsanvändning som inte ingår i det fasta priset. Varje dimension representerar en fakturerbar enhet. Det här är en variabel kostnad som ändras beroende på användningen av avgiftsmätta enheter, till exempel bandbredd, biljetter eller e-post som bearbetas. Du debiteras enligt din förbrukning av dessa dimensioner månadsvis. Observera att överförbrukning endast startar när du har använt alla enheter med dataförbrukning som ingår i det fasta priset.
- **Kostnadsfri utvärderingsversion** – i vissa fall innehåller planen en utvärderingsperiod på en månad, under vilken du kan använda programvaran kostnadsfritt.  När utvärderingsperioden är slut debiteras du enligt din plan. Utvärderingserbjudanden är inte kompatibla med anpassade mätare.

Dessa prissättningsmodeller är tillgängliga för både offentliga och privata planer.

## <a name="saas-purchase-experience"></a>SaaS-köpupplevelse

1. På produktsidan väljer du en plan som uppfyller dina behov och fortsätter att **konfigurera + prenumerera**
2. Som en del av inköpsprocessen **omdirigeras** du till fliken Grundläggande inställningar och du måste:
    1. Definiera vilken *prenumeration* du vill använda för fakturering. Den Azure-prenumeration som du använder bör ha en giltig inköpsmetod definierad för den. Du bör ha rätt behörighetsnivå eller ha en resursgrupp under prenumerationen med rätt behörighetsnivå. Faktureringsland bör också vara ett land där erbjudandet är tillgängligt för köp. Azure-prenumerationer utan giltig betalningsmetod (till exempel en MSDN-prenumeration) kan bara användas för att köpa kostnadsfria abonnemang
    1. Välj eller skapa en **resursgrupp som* SaaS-resursen ska tillhöra.
    1. Skriv ett *namn för* SaaS-prenumerationen så att du enkelt kan identifiera den senare. När du har köpt det kan du inte ändra namnet.
    1. Under **Plan** visas den plan som du valde på sidan med produktinformation (PDP). Om du inte har gjort ett aktivt val i PDP visas standardplanen. Du kan ändra ditt val genom att välja **länken Ändra** plan. Välj relevant faktureringsperiod och välj sedan en annan plan. Du kanske kan ändra planen efter köpet, om utgivaren stöder det. Du kommer dock inte att kunna ändra perioden från månadsvis till årlig eller från årlig till månatlig.
    1. I fall där prismodellen *är per* användare kan du behöva ange antalet *användare.* Priset som visas ändras baserat på den prenumeration, plan och period som du har valt.
3. Gå vidare **till** fliken Taggar *–* Taggar är användardefinierade nyckel/värde-par som kan placeras direkt på en resurs eller en resursgrupp. Du kan använda taggar för att enkelt hitta din SaaS-resurs senare. Azure stöder för närvarande upp till 50 taggar per resurs och resursgrupp. Taggar kan placeras på en resurs när den skapas eller läggas till i en befintlig resurs.
4. Fortsätt att **granska + prenumerera för** att gå igenom erbjudande- och planinformationen.
    1. Granska *Användningsvillkor,* *ändringar* och *sekretesspolicy för* utgivaren och även för Azure Marketplace
    1. Du kan bli ombedd att lägga till dina kontaktuppgifter
    1. Granska *information om grunder* *och* taggar
5. När du har bekräftat det väljer du **Prenumerera.**

## <a name="saas-subscription-and-configuration"></a>SaaS-prenumeration och konfiguration

När du väljer prenumerera visas meddelandet "Din SaaS-prenumeration pågår". Den här processen bör ta några minuter, stäng inte fönstret förrän det är klart.

När prenumerationen är klar visas ett meddelande om att saaS-prenumerationen har slutförts, och du bör konfigurera kontot så att du kan börja använda ditt köp. Du får också ett e-postmeddelande som ber dig att aktivera den nya prenumerationen. Om det inte är du som ska konfigurera SaaS-kontot vidarebefordrar du det här e-postmeddelandet till relevant person.

För att slutföra processen och börja använda SaaS måste du börja konfigurera din prenumeration. Genom att välja **knappen Konfigurera** konto nu omdirigeras du till utgivarens webbplats.

Du kan också kontrollera prenumerationsstatusen genom att välja klockikonen i det övre högra hörnet av rubriken.

Om du inte slutför konfigurationsprocessen inom *30 dagar* tas den här SaaS-prenumerationen *bort automatiskt.* Faktureringen startar när ditt konto har konfigurerats på utgivarens webbplats.

Felmeddelanden som du kan stöta på under processen:

- Det går *inte att köpa plannamnet för den* valda planen i en kostnadsfri prenumeration
  - Mer information finns i Uppgradera https://aka.ms/UpgradeFreeSub ditt konto.

- Köpet misslyckades eftersom det inte gick att hitta ett giltigt kreditkort eller en betalningsmetod som är associerad med din Azure-prenumeration.
  - Använd en annan Azure-prenumeration eller lägg till\uppdatera aktuellt kreditkort eller betalningsmetod för den här prenumerationen och försök igen.

- Plannamnet *på den plan som* valts  för erbjudandets namn efter utgivare av erbjudandet är inte tillgängligt för dig för köp enligt de regler som angetts av IT-administratören. 
  - Kontakta IT-administratören.

- Plannamnet *på den plan som*  valts av erbjudandeplanen som valts av utgivaren av erbjudandet är inte tillgängligt för köp på grund av privata Marketplace-inställningar som gjorts av din klients IT-administratör. 
  - Kontakta IT-administratören

- Köpet misslyckades eftersom den begärda faktureringsperioden är tom eller ogiltig.
  - Försök att köpa en annan plan/faktureringsperiod.

- Köpet misslyckades eftersom vi inte kunde verifiera din signering av ett juridiskt avtal.
  - Igen. Om felet kvarstår kan du försöka göra köpet med en annan Azure-prenumeration eller kontakta supporten.

- Det gick inte att *köpa offer offerID* av *utgivaren publisherID.* Det här erbjudandet är för närvarande inte tillgängligt för inköp.
  - Försök igen senare. Kontakta supporten om du fortsätter att få det här felmeddelandet efter en timme.  

- Det gick inte att  *köpa planID* för planID för erbjudandet *från utgivaren publisherID.* Den här planen är för närvarande inte tillgänglig för köp.
  - Försök igen senare. Kontakta supporten om du fortsätter att få det här felmeddelandet efter en timme. 

- Klientens *e-postadress* med objekt-ID *ObjectID* har inte behörighet att utföra åtgärden *DeploymentValidationAction* över omfånget *ResourceGroup; DeploymentScope* eller så är omfånget ogiltigt.  
  - Du får det här meddelandet om du inte har rätt behörigheter för Azure-prenumerationen/resursgruppen.  
    Uppdatera dina autentiseringsuppgifter om åtkomsten nyligen har beviljats.  
    Om du vill distribuera resurser till en resursgrupp måste du minst ha deltagaråtkomst. Kontrollera din åtkomststatus under **Resursgrupper** och välj **Access Control**. Detta visar vem "Ägare" är, som du kan be att tilldela dig som deltagare.

- Prenumerationen som används för det här köpet tillåter inte Marketplace-inköp.  
  - Använd en annan prenumeration eller be administratören att ändra definitionen för den här prenumerationen och försöka igen.

## <a name="next-steps"></a>Nästa steg

- Om du säljer ditt erbjudande via Microsoft går du till How to add a preview audience for your SaaS offer (Så här lägger du till en förhandsversion av ditt [SaaS-erbjudande).](/azure/marketplace/create-new-saas-offer-preview)
- Annars går du till [Så här säljer du ditt SaaS-erbjudande.](/azure/marketplace/create-new-saas-offer-marketing)
