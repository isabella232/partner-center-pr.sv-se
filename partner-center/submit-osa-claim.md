---
title: Skapa en kundassociation
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Skapa kundassociationer med Claiming Partner of Record -modellen (CPOR). Hjälper till att hantera försäljning, användning och incitament för Microsoft 365 & Dynamics 365-kunder.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 196009d9271324377be02d0b2d12ba8a4d7a993c
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960566"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a>Kundassociationer via CPOR-modellen (Claimed Partner of Record) för Microsoft 365 och Dynamics 365


**Lämpliga roller:** Incitamentsadministratör

Den 1 oktober 2019 började Microsoft använda CPOR-modellen (Claiming Partner of Record) för att hantera de associationer som du har med dina Microsoft 365- och Dynamics 365-kunder med avseende på Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 och OSU-Business Application incentives.

>[!Important]
> CPOR-anspråk (Customer Association) gäller endast för OSU(Online Services Sell, Online Services Usage) – Microsoft 365 och OSU-Business program. Om du skickar ett co-op-anspråk för ett annat program, till exempel Molnlösningsleverantör (CSP), Managed Reseller, värd eller Surface, kan du gå till Co-op-anspråksprocessen som beskrivs här. <br><br>När du skickar in ditt anspråk verifierar Microsoft det. Vi kan be dig om mer information i det här läget. Vi meddelar även kunden om din associationsbegäran. Kunder har fem arbetsdagar på sig att avanmäla sig. Om de inte avanmäler sig blir din koppling till den här specifika klientorganisationen och arbetsbelastningen officiell. Nu har du åtkomst till kundens användningsdata. 

Du behöver följande information för att slutföra ett anspråk:

- **MPN-ID** (Microsoft Partner Network-ID) för din entitet som gör anspråket

- Kundens domännamn **(mer information** finns i Hitta klientorganisations-ID, [domännamn, användarobjekt-ID](find-ids-and-domain-names.md))

- Kundens katalog-ID eller **klientorganisations-ID** (mer information finns i [Hitta klientorganisations-ID, domännamn, användarobjekt-ID](find-ids-and-domain-names.md)) 

- **Lösningsområdet,** till exempel Business Applications eller Microsoft 365

- Den **aktivitet** som du har utfört och vilken typ av anspråk du vill göra, till exempel förförsäljning, användning eller intäktsassociating

- Kundens kontaktnamn, **rubrik** och e-postadress

- För Dynamics 365 måste du också ange kundens tekniska **kontaktnamn,** titel och e-postadress

- Ditt eget företags **kontaktnamn och e-postadress**

- Du skapar ett namn **för det** här anspråket

- De **produkter eller** arbetsbelastningar som du begär

- **PoE (Proof of Execution),** till exempel en arbetsuttryck som signerats av kunden. Du kan också ladda ned en PoE-mall som du kan använda.

- För partner som endast begär intäktsassociation: **Dynamics-lösnings** säljarnamn, Kundnamn och **Namn på ISV-produkt/lösning**.  

Du bör också förstå följande:

- Om du har befintliga Microsoft 365-kunder måste du associera med dem som du vill fortsätta att skaffa OSU-incitament genom att använda den här processen.

- Om du har befintliga associationer med Dynamics 365 eller Power BI-kunder förblir dessa associationer giltiga fram till dess att prenumerationerna upphör att gälla.

- En kund kan ha flera partner, men varje arbetsbelastning (för OSU-Microsoft 365) eller prenumeration (för OSA-Sell- och OSU-Business-program) kan bara associeras med en partner.

## <a name="create-a-customer-association"></a>Skapa en kundassociation

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).

2. Välj fliken **Incitament,** välj **Översikt** och välj sedan **Kundassociationer.**

3. Längst upp på sidan Kundassociationer väljer du **+ Kundassociationer.**

4. Välj **MPN-ID** för den partnerplats som ska associeras med kunden och lägg sedan till kundens domännamn och katalog-ID. [Hitta det här](find-ids-and-domain-names.md)

5. Välj **Fortsätt**.

6. Välj **lösningsområdet** och **aktiviteten**. 

   >[!Note]
   >
   >Om du Business Applications väljer du **antingen Användning och/eller Förförsäljning** eller **Intäktsassociaty** och väljer sedan **Fortsätt.** 
   <br><br>Om du väljer Intäktsassociation får du ange lite annan information än vad som anges nedan.

7. Ange lämplig information på sidan **Associera** kund och välj sedan **Skapa anspråk.**

8. Välj de produkter som är associerade med den här kundassociatyten och välj sedan **Fortsätt.**

9. Fyll i kundens kontaktuppgifter och ditt företags kontaktuppgifter. Alla fält måste fyllas i. 

   >[!NOTE]
   >Om din produkt är Dynamics 365 och den produkt du väljer har flera prenumerationer för den här specifika kunden måste du också ange prenumerations-ID:t.

10. Ange din PoE. Du kan dra den till rutan, bläddra till din egen stöddokumentation eller använda en mall genom att välja **Ladda ned mall**. 

11. Lägg till och spara kommentarer om du vill och välj sedan **Skicka anspråk**. Vi skickar ett e-postmeddelande till kunden om att godkänna din kundassociation.

   >[!NOTE]
   >När du har skickat in din kundassociaty kan du inte redigera den.

Du ser status för kundassociationen i fältet **Status**.

Välj **Historik** om du vill visa historiken för en kundassociation.

## <a name="next-steps"></a>Nästa steg

- [Hantera kundassociationer](incentives-manage-customer-associations.md)